<template>
  <div class="head">
    <a class="download-pdf" @click="download">下载 PDF</a>
    <p class="last-modified">最后更新于2022年12月</p>
  </div>
</template>

<script>
// 页面导出为pdf格式 //title表示为下载的标题，html表示document.querySelector('#myPrintHtml')
import html2Canvas from 'html2canvas'
import JsPDF from 'jspdf'

export default {
  name: 'Head',
  data() {
    return {
      withList: {a3: {width: 297, height: 420}, a4: {width: 210, height: 297}}
    }
  },
  mounted() {
  },
  computed: {},
  methods: {
    download() {
      this.getPdf("张国毅 - 区块链开发工程师|全栈工程师", document.querySelector('.content'))
    },
    getPdf(title, html) {
      // console.log("html", html);
      const h3 = document.createElement('h3')
      h3.innerText = "本PDF文件生成自 http://www.guoyi.pro";
      h3.style.cssText = "padding: 10px;\n" +
        "    text-align: center;\n" +
        "    color: hsl(0deg 0% 0% / 15%);\n" +
        "    position: fixed;\n" +
        "    top: 60vh;\n" +
        "    left: calc(50vw - 350px);\n" +
        "    z-index: 11111111;\n" +
        "    font-size: 40px;\n" +
        "    transform: rotate(315deg);"

      //  reset this page scroll
      window.pageYOffset = 0;
      document.documentElement.scrollTop = 0
      document.body.scrollTop = 0

      //  targetDom - target 2 img
      const targetDom = html;
      //  copyDom - copy dom from targetDom
      const copyDom = html.cloneNode(true)
      //  init the copyDom
      copyDom.style.width = targetDom.scrollWidth + 'px'
      copyDom.style.height = targetDom.scrollHeight + 'px'
      copyDom.style.top = '0px'
      copyDom.style.zIndex = '-1'
      copyDom.appendChild(h3)

      //如果你的页面里有很多个“temp”类的话  感觉这种不太适合 “classArr ”取出的是类数组
      let classArr = copyDom.querySelectorAll(".animate__animated");
      for (let i = 0; i < classArr.length; i++) {
        const item = classArr[i];
        item.classList.remove("animate__animated");
      }

      let resumeDiv = document.querySelector('.resume-div');
      resumeDiv.appendChild(copyDom)

      // 使用html2canvas 转换html为canvas
      html2Canvas(copyDom, {
        allowTaint: true,
        taintTest: false,
        logging: false,
        useCORS: true,
        dpi: window.devicePixelRatio * 3, // 将分辨率提高到特定的DPI 提高四倍
        scale: 3, // 按比例增加分辨率
        windowWidth: 1920,
        windowHeight: copyDom.offsetHeight,
      }).then((canvas) => {
        var paper = "a4";
        var padding = 0;
        var paperSize = this.withList[paper];
        const pdf = new JsPDF('p', 'mm', paper) // A4纸，纵向
        const ctx = canvas.getContext('2d')
        const width = paperSize.width - padding * 2
        const height = paperSize.height - padding * 2; // A4大小，210mm x 297mm，四边各保留10mm的边距，显示区域190x277
        const imgHeight = Math.floor((height * canvas.width) / width) // 按A4显示比例换算一页图像的像素高度
        let renderedHeight = 0;
        console.log("canvas", canvas);
        while (renderedHeight < canvas.height) {
          const page = document.createElement('canvas')
          page.width = canvas.width
          page.height = Math.min(imgHeight, canvas.height - renderedHeight)

          // 用getImageData剪裁指定区域，并画到前面创建的canvas对象中
          page
            .getContext('2d')
            .putImageData(
              ctx.getImageData(
                0,
                renderedHeight,
                canvas.width,
                Math.min(imgHeight, canvas.height - renderedHeight)
              ),
              0,
              0
            )
          pdf.addImage(
            page.toDataURL('image/jpeg', 1.0),
            'JPEG',
            padding,
            padding,
            width,
            Math.min(height, (width * page.height) / page.width)
          ) // 添加图像到页面，保留 padding边距

          renderedHeight += imgHeight
          console.log(canvas.height, renderedHeight);
          if (renderedHeight < canvas.height) {
            pdf.addPage() // 如果后面还有内容，添加一个空页
          }
          // delete page;
        }
        // 保存文件
        pdf.save(`${title}.pdf`)
        copyDom.parentNode.removeChild(copyDom)
      })
    }
  }
}
</script>
<style lang="scss">
.head {
  .last-modified {

  }
}
</style>


