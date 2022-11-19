<template>
  <div class="content-bd">
    <div class="content-left">
      <section class="practice">
        <header class="section-hd">
          <span class="section-title-l"></span>
          <h2 class="section-title">项目经历</h2>
          <span class="section-title-r"></span>
        </header>
        <div class="section-bd">

          <!--经历:牙木科技股份有限公司-->
          <div class="item">
            <header class="item-hd">
              <img class="open" @click="openOrClose(0)"
                   :src="!open[0]?'static/jia-xianxingyuankuang.svg':'static/jian-xianxingyuankuang.svg'"/>
              <div class="company-des">
                <h3 class="item-name">牙木科技股份有限公司</h3>
                <span class="item-time">2022.03 至 今</span>
              </div>
              <a class="btn item-more"
                 href="https://baike.baidu.com/item/%E7%89%99%E6%9C%A8%E7%A7%91%E6%8A%80%E8%82%A1%E4%BB%BD%E6%9C%89%E9%99%90%E5%85%AC%E5%8F%B8/59098005?fr=aladdin"
                 target="_blank" title="点击查看->牙木科技股份有限公司百度百科">工作</a>
            </header>
            <ol :style="{display:(open[0]?'block':'none')}" class="item-project">
              <li class="project-1">
                <h3 class="project-name">
                  <a href="https://bitfactory.cn/" target="_blank"
                     title="点击进入->星火·链网首页">星火·链网 — BNS服务 [组长]</a></h3>

                <div class="div-project-item">
                  <h3 class="project-des">【项目简介】</h3>
                  <p class="item-project-des">
                    BNS（Beta Name
                    System）是星火链网原生的命名系统，基于星火·链网底层架构的名字服务系统，在唯一性、语义敏感的基础上，实现类似“自命名”的用户体验。任何人可获得自己想要的名字，应用于星火链网的各类型场景，包括但不限于NFT、数字身份，数字资产管理等。独立于ICANN/DNS名字空间，参考以太坊域名服务ENS等区块链名字服务，实现了人类可识别容易记住的。
                  </p>
                </div>
                <ol>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">智能合约核心服务开发</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>负责项目框架搭建以及疑难问题解决，为项目成员提供开发思路</li>
                          <li>主导整个项目正常开发流程，负责智能合约测试与审计</li>
                          <li>负责研究Ethereum 名字服务 ENS智能合约设计</li>
                          <li>负责实现BNS注册表核心合约</li>
                          <li>负责实现BNS用户多签投票合约</li>
                          <li>负责实现BNS名字注册、名字解析服务合约</li>
                          <li>负责实现BNS反向注册、反向解析服务合约</li>
                          <li>负责实现BNS注册管理委员会、业务资费服务合约</li>
                        </ul>
                      </div>
                    </div>
                  </li>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">引导前端开发Web3 DApp</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>主导整个项目正常开发流程，研究星火链网钱包插件及BIF.js使用方法</li>
                          <li>负责团队Web3应用开发引导，项目框架搭建以及疑难问题解决</li>
                        </ul>
                      </div>
                    </div>
                  </li>
                </ol>
              </li>

              <li class="project-1">
                <h3 class="project-name">
                  <a href="https://bitfactory.cn/" target="_blank"
                     title="点击进入->星火·链网首页">星火·链网 — DID服务 [核心开发]</a></h3>

                <div class="div-project-item">
                  <h3 class="project-des">【项目简介】</h3>
                  <p class="item-project-des">
                    DID（Decentralized
                    Identifier，去中心化身份体系），作为一种新的身份标识，由传统的中心化身份衍化和派生出来，指去中介化，个人或组织完全拥有的自身数字身份的所有权，控制权以及管理权，将这部分权利完全归于用户自身。
                  </p>
                </div>
                <ol>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">智能合约核心服务开发</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>负责项目框架搭建以及疑难问题解决，为项目成员提供开发思路</li>
                          <li>主导整个项目正常开发流程，负责智能合约测试与审计</li>
                          <li>负责实现DID链上解析核心合约</li>
                          <li>负责实现DID用户多签投票合约</li>
                          <li>负责实现DID预言机链下解析合约</li>
                        </ul>
                      </div>
                    </div>
                  </li>
                </ol>
              </li>

              <li class="project-1">
                <h3 class="project-name">
                  <a href="https://bitfactory.cn/" target="_blank"
                     title="点击进入->星火·链网首页">星火·链网 — 新型标识管理体系 [核心开发]</a></h3>

                <div class="div-project-item">
                  <h3 class="project-des">【项目简介】</h3>
                  <p class="item-project-des">
                    新型标识管理体系基于星火链网提供的BID和智能合约，根据新型标识治理体系中对于标识数据（包括DNS，从广义角度看DNS也可以作为一种标识看待，如无特殊说明后续文档中所述的标识均包括DNS）管理的设计，通过个标识联盟委员会、安全稳定委员会和投票机制等保障标识数据的安全、公平管理，有效解决了传统标识根解析体系中存在的弊端。
                  </p>
                </div>
                <ol>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">智能合约核心服务开发</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>负责项目框架搭建以及疑难问题解决，为项目成员提供开发思路</li>
                          <li>主导整个项目正常开发流程，负责智能合约测试与审计</li>
                          <li>负责实现标识业务管理器、标识数据注册及解析器核心合约</li>
                          <li>负责实现标识管理用户多签投票合约</li>
                          <li>负责实现DNS标识预言机</li>
                        </ul>
                      </div>
                    </div>
                  </li>
                </ol>
              </li>
            </ol>
          </div>

          <!--经历:公链开发项目-->
          <div class="item">
            <header class="item-hd">
              <img class="open" @click="openOrClose(1)"
                   :src="!open[1]?'static/jia-xianxingyuankuang.svg':'static/jian-xianxingyuankuang.svg'"/>
              <div class="company-des">
                <h3 class="item-name">Web3工作室</h3>
                <span class="item-time">2021.03 至 2022.03</span>
              </div>
              <a class="btn item-more" target="_blank" title="点击查看->牙木科技股份有限公司百度百科">工作</a>
            </header>
            <ol :style="{display:(open[1]?'block':'none')}" class="item-project">
              <li class="project-1">
                <h3 class="project-name">
                  <a href="https://bitfactory.cn/" target="_blank"
                     title="点击进入->星火·链网首页">BSC链 — NFT交易所 [组长]</a></h3>

                <div class="div-project-item">
                  <h3 class="project-des">【项目简介】</h3>
                  <p class="item-project-des">
                    NFT，全称为Non-Fungible Token，指非同质化通证，实质是区块链网络里具有唯一性特点的可信数字权益凭证，是一种可在区块链上记录和处理多维、复杂属性的数据对象。
                    本项目提供了一个去中心化的数字藏品交易平台。
                  </p>
                </div>
                <ol>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">智能合约核心服务开发</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>负责项目框架搭建以及疑难问题解决，为项目成员提供开发思路</li>
                          <li>主导整个项目正常开发流程，负责智能合约测试与审计</li>
                          <li>负责研究Ethereum opensea智能合约设计</li>
                          <li>负责实现NFT发布及交易买卖核心合约</li>
                        </ul>
                      </div>
                    </div>
                  </li>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">主导开发NFT交易所前端</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>主导整个项目正常开发流程，研究metamask钱包插件及web3.js使用方法</li>
                          <li>负责团队Web3应用开发引导，项目框架搭建以及疑难问题解决</li>
                          <li>负责开发核心NFT交易模块</li>
                        </ul>
                      </div>
                    </div>
                  </li>
                </ol>
              </li>

              <li class="project-1">
                <h3 class="project-name">
                  <a href="https://bitfactory.cn/" target="_blank"
                     title="点击进入->星火·链网首页">以太坊 — 去中心化链上资管平台 [组长]</a>
                </h3>

                <div class="div-project-item">
                  <h3 class="project-des">【项目简介】</h3>
                  <p class="item-project-des">
                    传统金融项目中的资金管理一般使用银行网银、支付宝、微信等，但存在平台倒闭用户对自己资金不能掌控的问题；在中心化交易所中，用户资金由平台方保管，但交易所平台存在挪用资金的可能性，不能保证用户资金的透明。本系统通过智能合约合同开源代码管理用户资金，解决了平台对用户热钱的去中心化管控，实现了用户资金的透明化管理。
                  </p>
                </div>
                <ol>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">智能合约核心服务开发</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>负责项目框架搭建以及疑难问题解决，为项目成员提供开发思路</li>
                          <li>主导整个项目正常开发流程，负责智能合约测试与审计</li>
                          <li>负责实现链上资金存储、提取核心合约</li>
                          <li>负责实现平台管理员多签投票管理资金合约</li>
                          <li>负责实现链上链下交互的预言机合约</li>
                        </ul>
                      </div>
                    </div>
                  </li>
                </ol>
              </li>

              <li class="project-1">
                <h3 class="project-name">
                  <a href="https://bitfactory.cn/" target="_blank"
                     title="点击进入->星火·链网首页">以太坊 — 去中心化组织自治系统（DAO） [组长]</a></h3>

                <div class="div-project-item">
                  <h3 class="project-des">【项目简介】</h3>
                  <p class="item-project-des">
                    传统系统核心管理员拥有着极高的中心化权限，但我们可以通过去中心化自治系统实现用户真正的当家做主，可以实现对小区物业管控、核心业务投票表决、新需求投票评审等功能。
                  </p>
                </div>
                <ol>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">智能合约核心服务开发</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>负责项目框架搭建以及疑难问题解决，为项目成员提供开发思路</li>
                          <li>主导整个项目正常开发流程，负责智能合约测试与审计</li>
                          <li>负责实现去中心化多签投票核心合约</li>
                          <li>负责实现去中心化业务管理合约</li>
                        </ul>
                      </div>
                    </div>
                  </li>
                </ol>
              </li>
              <li class="project-1">
                <h3 class="project-name">
                  <a href="https://bitfactory.cn/" target="_blank"
                     title="点击进入->星火·链网首页">蚂蚁联盟链 — 基于区块链的农产品溯源平台 [组长]</a></h3>

                <div class="div-project-item">
                  <h3 class="project-des">【项目简介】</h3>
                  <p class="item-project-des">
                    目前人们越来越注重生活品质，注重农产品食品安全；本项目通过区块链对农产品生产过程实时上链，保证数据可靠、可信、可追溯。
                  </p>
                </div>
                <ol>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">核心业务模块开发</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>负责项目框架搭建以及疑难问题解决，为项目成员提供开发思路</li>
                          <li>主导整个项目正常开发流程，负责智能合约测试与审计</li>
                          <li>负责实现去中心化农产品生产数据上链核心合约</li>
                          <li>负责实现链下传感器数据采集服务，实现生产环节管理服务</li>
                        </ul>
                      </div>
                    </div>
                  </li>
                </ol>
              </li>
            </ol>
          </div>
          <!--经历:绿豆芽科技-->
          <div class="item">
            <header class="item-hd">
              <img class="open" @click="openOrClose(2)"
                   :src="!open[2]?'static/jia-xianxingyuankuang.svg':'static/jian-xianxingyuankuang.svg'"/>
              <div class="company-des">
                <h3 class="item-name">西安绿豆芽信息科技有限公司</h3>
                <span class="item-time">2017.08 至 2020.02</span>
              </div>
              <a class="btn item-more"
                 href="https://baike.baidu.com/item/%E8%A5%BF%E5%AE%89%E7%BB%BF%E8%B1%86%E8%8A%BD%E4%BF%A1%E6%81%AF%E7%A7%91%E6%8A%80%E6%9C%89%E9%99%90%E5%85%AC%E5%8F%B8"
                 target="_blank" title="点击查看->西安绿豆芽信息科技有限公司百度百科">工作</a>
            </header>
            <ol :style="{display:(open[2]?'block':'none')}" class="item-project">
              <li class="project-1">
                <h3 class="project-name">
                  <a href="http://www.bitchang.com" target="_blank"
                     title="点击进入->币厂交易所首页">数字货币交易所 [组长]</a></h3>
                <div class="div-project-item">
                  <h3 class="project-des">【项目简介】</h3>
                  <p class="item-project-des">
                    该项目为数字货币交易所，为用户提供便捷的数字资产交易系统，包括币币交易、法币交易、行情查看等主要功能。后端开发语言采用Java，主要采用Spring boot + Hibernate
                    JPA作为后端服务框架；项目后端服务主要包含：API网关、JWT用户认证、去中心化钱包的资金管理、交易系统、交易订单撮合引擎、WebSocket
                    K线数据分发服务以及钱包系统（区块链链上操作）等多项服务组成。</p>
                </div>
                <ol>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">交易所后端</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>负责项目框架搭建以及疑难问题解决，为项目成员提供开发思路</li>
                          <li>主导整个项目正常开发流程，研究了高可用、高并发服务器的架构设计（keepalived+nginx+haproxy）</li>
                          <li>对常用数据进行缓存处理（Redis），并对[撮合引擎]系统进行了架构设计，采用Redis内存撮合、Rabbit MQ消息队列异步入库实现高性能撮合系统，从而实现撮合引擎弹性伸缩
                          </li>
                          <li>
                            针对Redis可能出现脏读的问题可以采用消息队列处理，消除多线程同一时间操作同一Redis数据的脏读问题；或可以通过Redis锁解决高并发的脏读问题（不推荐，可能会造成无效等待）
                          </li>
                        </ul>
                      </div>
                    </div>
                  </li>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">交易所前端</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>该项目前端开发框架采用目前市面流行的Vue.js框架与Element UI 2.0。采用websocket、TradingView、vuex等技术栈</li>
                          <li>负责项目框架搭建以及疑难问题解决，为项目成员提供开发思路</li>
                          <li>主导整个项目正常开发流程，研究K线渲染组件TradingView的使用与原理</li>
                          <li>负责Android端APP基础框架搭建，采用xUtils进行网络请求、websocket进行实时数据传输</li>
                        </ul>
                      </div>
                    </div>
                  </li>
                  <li class="project-2">
                    <div class="item-bd">
                      <h3 class="project-name-2">以太坊智能合约开发</h3>
                      <div class="div-item">
                        <h3 class="project-des">【工作职责】</h3>
                        <ul class="section-content">
                          <li>在法律允许范围内，负责公司在数字货币、智能合约开发上的需求</li>
                          <li>负责多账户签名合约设计与开发</li>
                          <li>负责智能合约审计及测试</li>
                        </ul>
                      </div>
                    </div>
                  </li>
                </ol>
              </li>
              <li class="project-1">
                <h3 class="project-name">
                  <a href="http://www.bitchang.com" target="_blank"
                     title="点击进入->数字货币钱包">数字货币钱包 [核心开发]</a>
                </h3>
                <div class="div-project-item">
                  <h3 class="project-des">【项目简介】</h3>
                  <p class="item-project-des">
                    该项目是一款加密数字货币钱包项目，为用户提供去中心化区块链数字货币钱包功能，包含：转账、收付款、资产查看、合约挖矿、共振等功能。主要涉及区块链链上交易发起及获取链上数据、合约挖矿订单等操作
                  </p>
                </div>
                <div class="div-project-item">
                  <h3 class="project-des">【工作职责】</h3>
                  <ul class="section-content">
                    <li>负责项目框架搭建以及链上交互开发</li>
                    <li>通过公链提供API以及JSON RPC文档实现数字货币转账、充提币、钱包创建等逻辑</li>
                  </ul>
                </div>
              </li>
            </ol>
          </div>

          <!--经历:在校-->
          <div class="item">
            <header class="item-hd">
              <img class="open" @click="openOrClose(3)"
                   :src="!open[3]?'static/jia-xianxingyuankuang.svg':'static/jian-xianxingyuankuang.svg'"/>
              <div class="company-des">
                <h3 class="item-name">校内创业工作室</h3>
                <span class="item-time">2015.08 ~ 2017.08</span>
              </div>
              <a class="btn item-more" href="http://www.ztbu.edu.cn/" title="河南理工大学万方科技学院官网">在校</a>
            </header>
            <div :style="{display:(open[3]?'block':'none')}" class="item-bd">
              <p class="item-des">在校期间创建工作室，担任技术总监主导和带领朋友创业，工作室曾服务于：<span style="font-weight: bold">高校、企业及个人</span>，部分项目如下：
              </p>
              <ul class="section-content">
                <li><a href="http://tw.ztbu.edu.cn/" target="_blank" title="点击进入->校团委官网">校团委官网</a>
                  学院组织年度网页设计开发比赛，作为胜出团队有偿开发并维护校团委官网
                </li>
                <li><a href="https://www.beious.com/" target="_blank" title="点击进入->贝欧名邸官网">贝欧名邸家具</a> 湖南全屋定制家具客户公司商城系统
                </li>
                <li><a href="https://android.myapp.com/myapp/detail.htm?apkName=com.fendoumao.waimai"
                       target="_blank" title="点击查看->奋斗猫APP">奋斗猫APP</a>
                  西安客户公司APP外卖点餐系统
                </li>
                <li>
                  <a href="https://baike.baidu.com/item/%E5%A5%8B%E6%96%97%E7%8C%AB" title="点击查看->奋斗猫百度百科">奋斗猫全网优化</a>
                  奋斗猫全网优化项目包含搜索引擎优化（SEO）
                </li>
              </ul>
            </div>
          </div>
        </div>
      </section>
    </div>
    <div class="content-right">
      <section class="skill">
        <header class="section-hd">
          <span class="section-title-l"></span>
          <h2 class="section-title">技能</h2>
          <span class="section-title-r"></span>
        </header>
        <div class="section-bd">

          <!--技能:区块链开发-->
          <div class="item">
            <header class="item-hd">
              <span class="item-time">区块链 | Web3 | 智能合约</span>
              <a class="btn item-more-right">熟练掌握</a>
            </header>
            <div class="item-bd">
              <ul class="section-content">
                <li>拥有五年区块链行业开发经验，涉及 中心化虚拟货币交易所、DEX、Web 3.0
                  DAPP、DEFI、区块链存证、电子合同（智能合约）、链游、NFT、区块链钱包、DAO等应用方向，掌握去中心应用开发思维
                </li>
                <li>熟练掌握ERC20、ERC721、ERC1155等合约标准，有流动性挖矿、DEX、借贷、Token、DAO、NFT等智能合约开发经验，熟练掌握Web3 DAPP开发逻辑，熟悉常见智能合约漏洞</li>
                <li>熟练使用Solidity语言，熟练使用JavaScript、web3.js、web3J、tron4J；正学习Rust等开发语言</li>
                <li>熟悉Solidity开发和优化，熟悉Truffle、Remix等开发工具，熟悉OpenZeppelin等三方安全合约库；</li>
                <li>
                  理解比特币、以太坊、Polkadot、BSC、TRON、Polygon、Solana、IPFS等区块链公链的运行逻辑，掌握公网节点的搭建及私链网络的搭建；有蚂蚁联盟链、星火链网、BSN等联盟链3年应用开发经验
                </li>
                <li>理解以太EVM原理，熟悉区块链算法，共识机制，安全协议，智能合约等底层协议与运行机制；</li>
                <li>熟悉主流DeFi协议，如Uniswap/1inch/MakerDao/Compound等</li>
                <li>熟悉主链NFT交易所逻辑，如Opensea，Apenft等</li>
                <li>有金融交易、区块链及数字货币行业独立工作经验</li>
              </ul>
            </div>
          </div>

          <!--技能:WEB后端开发-->
          <div class="item">
            <header class="item-hd">
              <span class="item-time">WEB后端开发</span>
              <a class="btn item-more-right">熟练掌握</a>
            </header>
            <div class="item-bd">
              <ul class="section-content">
                <li>五年后端应用Java、PHP实际开发经验，掌握Java面向对象思想编程</li>
                <li>熟练使用Spring Boot、SpringMVC等主流框架，熟悉Restful 风格API设计</li>
                <li>熟练使用数据库操作框架Hibernate JPA，掌握SQL语句增删改查</li>
                <li>熟练使用Websocket，并使用websocket进行服务端与客户端实时数据传输</li>
                <li>熟练使用Jwt等用户鉴权产品</li>
                <li>熟悉API开发基本流程，熟悉Restful 风格API设计</li>
                <li>熟练使用非关系型数据库Redis、MongoDB等，有Redis实际项目开发使用经验</li>
                <li>熟练使用消息中间件Rabbit MQ、kafka等开源中间件，有Rabbit MQ实际项目开发使用经验</li>
                <li>了解Spring cloud，正学习Spring cloud在企业大型应用中的应用，以及大型应用的微服务化及服务治理知识学习</li>
                <li>有金融交易、区块链及数字货币行业独立工作经验</li>
              </ul>
            </div>
          </div>

          <!--React-->
          <div class="item">
            <header class="item-hd">
              <span class="item-time">数据库</span>
              <a class="btn item-more-right">熟练掌握</a>
            </header>
            <div class="item-bd">
              <ul class="section-content">
                <li>熟悉关系型数据库技术，熟练使用关系型数据库Mysql、Oracle</li>
                <li>熟悉非关系型数据库技术，熟练使用非关系型数据库Nosql：Redis</li>
                <li>熟练使用Hibernate JPA，了解 MyBatis、JDBC等数据库操作框架使用</li>
                <li>了解分布式数据库及Mycat中间件，并正致力于提高分布式数据库能力和对于数据库高并发高可用的知识储备</li>
              </ul>
            </div>
          </div>

          <!--服务器|架构-->
          <div class="item">
            <header class="item-hd">
              <span class="item-time">服务器|架构</span>
              <a class="btn item-more-right">熟练掌握</a>
            </header>
            <div class="item-bd">
              <ul class="section-content">
                <li>熟练掌握Nginx、Tomcat、Apache服务器使用</li>
                <li>熟练掌握常用软件（MySQL、Redis、Rabbit MQ等）在服务器的搭建与使用</li>
                <li>熟练使用Centos(Linux)云服务器并掌握线上环境和应用的部署</li>
                <li>了解Docker使用及Docker应用部署</li>
                <li>熟悉微服务、高并发、高可用集群服务端架构</li>
                <li>熟练掌握Git、Github、gradle、maven等工具使用</li>
              </ul>
            </div>
          </div>

          <!--WEB前端开发-->
          <div class="item">
            <header class="item-hd">
              <span class="item-time">WEB前端开发</span>
              <a class="btn item-more-right">掌握</a>
            </header>
            <div class="item-bd">
              <ul class="section-content">
                <li>有一年以上Android原生开发经验，熟练掌握使用Java SE开发Android原生APP</li>
                <li>熟悉前端技术HTML、VUE、JS、CSS、Flutter，有实际项目中的前端开发、维护经验</li>
                <li>掌握网页重构所需的CSS、SCSS</li>
                <li>掌握前端流行框架Vue、element UI</li>
                <li>熟知JS基本语法与知识，熟悉JS语法</li>
                <li>熟练使用Websocket，并使用其进行服务端与客户端实时数据传输</li>
                <li>熟练使用Tradingview，使用Tradingview进行K线展示</li>
              </ul>
            </div>
          </div>

          <!--Golang-->
          <div class="item">
            <header class="item-hd">
              <span class="item-time">Golang</span>
              <a class="btn item-more-right">了解</a>
            </header>
            <div class="item-bd">
              <ul class="section-content">
                <li>熟悉Golang基本语法与标准库</li>
                <li>用Golang开发过小型项目服务</li>
              </ul>
            </div>
          </div>

          <!--独立开发-->
          <div class="item">
            <header class="item-hd">
              <span class="item-time">独立开发</span>
            </header>
            <div class="item-bd">
              <ul class="section-content">
                <li>有独自主导并负责的项目开发经验，在项目中可进行独立开发</li>
                <li>有良好的编码习惯与编程思想，学习能力强，可快速学习新技术，对新技术、好技术热爱</li>
                <li>工作稳定性高，对公司负责，有一定的项目管理经验，有创业经历</li>
              </ul>
            </div>
          </div>

          <!--其它-->
          <div class="item">
            <header class="item-hd">
              <span class="item-time">其它</span>
            </header>
            <div class="item-bd">
              <ul class="section-content">
                <li>掌握Java、PHP、Golang、C、Git、Docker、硬件开发</li>
                <li>本科毕设：智能家电物联网控制系统</li>
                <li>资深Mac & JetBrains用户</li>
              </ul>
            </div>
          </div>
        </div>
      </section>

      <!--开源项目-->
      <section class="project">
        <header class="section-hd">
          <span class="section-title-l"></span>
          <h2 class="section-title">开源/项目</h2>
          <span class="section-title-r"></span>
        </header>
        <div class="section-bd">
          以下是我的开源项目与学习总结，细节请点击链接查看文档（其他项目开发中，尚未开源，敬请期待）

          <!--项目:博客-->
          <div class="item">
            <header class="item-hd">博客 & Github</header>
            <div class="item-bd">
              <ul>
                <li>
                  <a href="https://web3dapp.blog.csdn.net/" target="_blank">我的博客</a>
                </li>
                <li>
                  <a href="https://github.com/GuoyiZhang" target="_blank">Github</a>
                </li>
                <li>
                  <a href="http://www.guoyi.pro" target="_blank">个人网站主页</a>
                </li>
              </ul>
            </div>
          </div>

          <!--项目:WEB前端-->
          <div class="item">
            <header class="item-hd">开源项目</header>
            <div class="item-bd">
              <ul>
                <li>
                  <a href="https://github.com/GuoyiZhang/078-Vue-resumeVue" target="_blank">个人简历Vue</a>一份优雅简约的简历VUE版本
                </li>
                <li>
                  <a href="https://github.com/GuoyiZhang/082-BlogToMarkdown" target="_blank">博客导出为markdown</a>将Html版本的网页导出为markdown格式文档
                </li>
                <li>
                  <a href="https://github.com/GuoyiZhang/015-Java_Server-qiniuCommon" target="_blank">七牛云上传</a>
                </li>
                <li>
                  <a href="https://github.com/GuoyiZhang/013-HtmlWeb-Js_KLine" target="_blank">K线</a>
                  JS实现的K线展示组件，项目基于开源项目改造
                </li>
                <li>
                  <a href="https://github.com/GuoyiZhang/077-Android-ListeningLove" target="_blank">乐听乐爱APP</a>
                  全网音乐搜索与播放APP，可播放下载酷狗、QQ音乐、网易云等音乐库资源，此项目仅用于学习交流
                </li>
                <li>
                  <a href="#" target="_blank">虚拟货币钱包</a> 暂未开源
                </li>
                <li>
                  <a href="#" target="_blank">NFT交易所</a> 暂未开源
                </li>
                <li>
                  <a href="#" target="_blank">DAO去中心化自治项目</a> 暂未开源
                </li>
                <li>
                  <a href="#" target="_blank">Defi项目导航</a> 暂未开源
                </li>
              </ul>
            </div>
          </div>
        </div>
      </section>

      <!--奖项/证书-->
      <section class="prize">
        <header class="section-hd">
          <span class="section-title-l"></span>
          <h2 class="section-title">奖项/证书</h2>
          <span class="section-title-r"></span>
        </header>
        <div class="section-bd">

          <!--技能:WEB后端开发-->
          <div class="item">
            <header class="item-hd">
              <span class="item-time">获奖经历</span>
            </header>
            <div class="item-bd">
              <ul class="section-content">
                <li>2017年9月获得Ican创新设计大赛三等奖</li>
                <li>2017年7月获得智能互联创新大赛二等奖</li>
                <li>2016年获得校网页设计大赛三等奖</li>
                <li>2016年获得计算机二级证书</li>
              </ul>
            </div>
          </div>
        </div>
      </section>

      <!--致谢-->
      <section class="thanks">
        <header class="section-hd">
          <span class="section-title-l"></span>
          <h2 class="section-title">致谢</h2>
          <span class="section-title-r"></span>
        </header>
        <div class="section-bd">
          <!--技能:WEB后端开发-->
          <div class="item">
            <h2 style="font-weight: bold;line-height: 24px;margin-top: 10px">
              感谢您在百忙之中阅读这份履历，诚挚的期望能得到面试的机会，希望有荣幸能为公司效力！再次致以我最诚挚的谢意！！</h2>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
import $ from 'jquery'

export default {
  name: 'Content',
  components: {},
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
      open: [true, true, false, false, false, false],
    }
  },
  mounted() {
    $(document).ready(function () {
      if ($('ol:first').css('list-style-type') == 'none') { /* For IE6/7 only. */
        $('ol ol').each(function (i, ol) {
          ol = $(ol);
          var level1 = ol.closest('li').index() + 1;
          ol.children('li').each(function (i, li) {
            li = $(li);
            var level2 = level1 + '.' + (li.index() + 1);
            li.prepend('<span>' + level2 + '</span>');
          });
        });
      }
    });
  }, methods: {
    openOrClose(id) {
      this.open[id] = !this.open[id];
      console.log(this.open[id]);
      this.$forceUpdate();
    },

  }
}
</script>
