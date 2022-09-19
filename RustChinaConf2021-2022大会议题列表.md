# RustChinaConf 2021~2022大会议题列表



# 主会场



## Rustdoc: 你可以用它做什么，以及它的未来

Guillaume Gomez，华为工程师，rustdoc团队负责人。我的最终目标是使文档的编写尽可能简单，以便所有项目都有很好的文档

Rustdoc是官方的Rust工具，可以为你的crates生成文档。但它所做的远不止这些：它允许你测试你的代码示例，在文档和项目的源代码之间切换，将markdown文件转换为HTML，自动生成项目的链接，显示文档的覆盖范围，它有自己的行数，它允许，等等。

但这还不是全部! 很多更美好的功能即将到来。例如，其中一个功能允许你从源代码页面直接跳到一个项目的定义或其文档页面。

本讲座将介绍这些功能，让你了解rustdoc允许你做什么。

 Guillaume Gomez, a Huawei engineer and the rustdoc team leader. My end goal is to make documentation as simple as possible to write so that all projects have great docs!

Rustdoc is the official Rust tool to generate documentation for your crates. But it does much more than this: it allows you to test your code examples, to switch between the documentation and the source code of an item, to convert markdown file into HTML, to automatically generates links to items, to show the documentation coverage, it has its own lints, it allows, etc.

But this isn’t everything! A lot of even nicer feature are coming! For example, one of them allows you to directly jump to the definition of an item or its documentation page from the source code pages!

This talk will go through them to give you an idea what rustdoc allows you to do!

##  Rust 计算加速技术解读及高性能代码重构实践 

李原，2020年毕业于北京航空航天大学，同年加入华为开源能力中心。目前主要参与Rust语言核心技术贡献，是社区roadmap级特性stdsimd计算加速库的主力贡献者，并受社区member邀请成为ARM SIMD特性reviewer。专注于Rust编译器、数学算法、软硬件协同调优领域的研究，在Rust官方SIMD社区及数学库ndarray社区皆为Top5贡献者，并持续参与Rust社区编译器、语言、基础库方向的贡献。

运营效率是评价程序和编程语言时的重要考量，而单指令多数据流(SIMD)是一种能显著提升程序效率的计算加速技术。本议题会以该技术为核心，从社区贡献者的角度介绍Rust社区中计算加速库的发展及现状，并以实际开发中的代码重构案例实践为基础，为大家解读Rust中各种计算加速技术的使用，希望能对大家平时的学习和开发有所启示。



## 从零开始实现Rust Fuzzer

讲师： 陈鹏 ， 腾讯安全大数据实验室安全研究员，曾开发Angora、Matryoshka等多个模糊测试工具，在IEEE S&P, ACM CCS, Usenix Security等安全顶级会议发表多篇论文。

模糊测试(Fuzzing)是一种高效的自动化漏洞挖掘手段，其本身的实现需要高效的执行效率和高度抽象的输入，我们将介绍使用Rust来实现模糊测试工具核心特性时遇到的挑战，以及如何解决的它们的。

 复杂 Rust 开源项目的维护

讲师：Robert Yan，NEAR Proctol 工程师

维护一个复杂的 Rust 项目会遇到各类挑战。本次演讲介绍维护一个10~20万行代码级别的 Rust 区块链项目时，在架构、workspace、编译、测试等方面的经验和心得。

## 复杂 Rust 开源项目的维护

讲师：Robert Yan，NEAR Proctol 工程师

维护一个复杂的 Rust 项目会遇到各类挑战。本次演讲介绍维护一个10~20万行代码级别的 Rust 区块链项目时，在架构、workspace、编译、测试等方面的经验和心得。



## 圆桌会议： Rust 中国开源力量

自 Rust 1.0 以来，Rust 在中国就点燃了星星之火，来自中国的为 Rust 社区做贡献的开源贡献者有很多很多。如果有可能，我们希望可以邀请他们每个人都来分享他们与 Rust 的故事。包括我们大会的每位讲师，有很多人都为 Rust 开源社区做了很多贡献。
可惜时间有限，我们只能邀请三位在开源社区比较有突出贡献的三位嘉宾来给大家分享他们与 Rust 的故事。 

嘉宾：

- 孙黎，社区id：老油条，Async-graphql/Poem框架作者
- 洛佳，华中科技大学网络空间安全学院大四学生，RustSBI 作者
- 朱霜，Rust Search Extension 和 2d2d.io 作者/字节跳动工程师









# 分会场 1  Rust 语言研究与应用

## 基于LLVM Rust代码混淆设计与实现

赵禅， 蚂蚁集团 基础安全部 安全专家

本分享介绍如何基于 LLVM 为 Rust 代码进行混淆，并且分享一些案例。

## Rust API可靠性分析与验证

姜剑峰，复旦大学计算机学院硕士在读，现在在蚂蚁集团安全计算部门实习。目前的关注方向是通过验证工具以及程序分析的手段来保证Rust程序的可靠性。

模糊测试（fuzz）是一种有力的寻找程序错误的手段。模糊测试以随机或者启发式的方法产生大量输入，进而反复执行程序来检测程序中的错误。Rust模糊测试有一个活跃的社区，已经通过实践证明了模糊测试在Rust开源项目上寻找程序错误的能力。本talk将和大家分享Rust模糊测试技术的背景，适用场景，以及我们关于如何自动为Rust库生成模糊测试目标程序的初步的研究结果。

## 你为什么需要「Rust 编码规范」

张汉东，独立企业咨询师，国内Rust 布道者和中文社区的开拓者，著有《Rust编程之道》。

本次分享将带你整体认识《Rust 编码规范》，以及如何在项目中应用编码规范。 

你可能也会有以下疑问： 

1. 为什么 Rust 语言有严格的编译器检查和clippy这样的静态检查工具还需要编码规范？ 
2. Rust 编码规范的立意和目标是什么样的？
3. Rust 编码规范和 Clippy 之类的工具是什么关系？
4. Rust 编码规范内容组织是怎么样的？
5. 如何在项目中应用 Rust 编码规范？

或者其他一些疑问，在本次分享会中都可以得到解答，欢迎参与。



# 分会场2 ： Rust 拓展与优化

## 我们如何通过手工汇编代码击败 Rust 的零成本抽象

叶万标，具有十多年经验的高度专注的软件工程师, 使用各种技术在多种开发和工程职位中.  在业余时间, 我喜欢探索老旧的技术, 从纸带程序开始, 第一枚商用处理器到最古老的游戏机. 从前人的智慧中获取灵感, 并指导如今的程序开发. 这是一个有趣的体验, 因为你能学到许多极端的改善性能的方案.

ckb-vm 是 Rust 实现的 RISC-V 虚拟机, 我们通过在其关键位置引入手工汇编代码以获得相较原生 Rust 代码 5 倍以上的性能提升.

##  通过 Rust 拓展 js 并在 WebAssembly 中运行

陈思衡，WasmEdge 工程师。喜欢用技术让生活变得更美好。

WebAssembly (Wasm) 最初为浏览器应用而生，但随着 WASI 的出现以及开发者生态的壮大，Wasm 作为一种轻量级的软件容器在服务端的作用愈发明显。服务端的 Wasm 提供了与本地代码相媲美的速度，但又不失安全性，可移植性，与可管理性。 通过支持 JavaScript 在 wasm 中运行，可以绕开学习  c/c++、rust 使得开发者可以对基于 wasm 的产品有流畅的上手体验，减少因为开发语言的问题而流失用户的遗憾。 得益于 Rust 优秀的设计，使用 Rust 来拓展 JavaScript runtime 能够开发出高质量的 module，给用户稳定的使用体验。

## 定制你的 Future executor

讲师介绍：陈奕霖，PingCAP 研发工程师，TiKV committer，tikv/yatp 作者。

经过多年的发展，async Rust 生态逐渐成熟。绝大多数开发者会使用流行的 async runtime（如 tokio）作为 Future executor. 但 tokio 作为一个普适的 async runtime，不一定能最完美地实现每个项目的具体需求。本次演讲将以 TiKV 为例，谈谈如何定制自己的 Future executor，实现性能指标收集、高级调度控制、动态线程数调整等高级特性。






# 分会场 3 ： Rust  商业实践

## 云原生区块链框架实践之路

宁志伟

溪塔科技联合创始人兼首席架构师。前阿里巴巴底层架构师，参与Open JDK发行版本《龙井》，前华为OS团队架构师，领导团队支持海思首款ARM芯片，超过10年分布式系统架构设计，编程语言和虚拟机方面工作经验。首个微服务架构区块链CITA首席架构师，首个云原生区块链 CITA-Cloud 框架设计者。Rustcon Asia 演讲嘉宾。开源社区CITAHub联合发起人。OSCHINA 讲师。国内第一个公开发布的跨链协议——《陆羽跨链协议（Luyu Cross Chain Protocol）》联合发起人之一。

内容介绍：

随着云原生技术的普及，使用云原生技术栈来迭代发布应用已经成为常态。云原生和区块链两种技术都属于分布式系统的范畴，区块链的去中心化和可信计算的特质，能够在实际应用中弥补云原生的不足。本篇将从主要特性、微服务架构、运维部署等方面一一阐述云原生区块链框架的实践之路。

##  我们能从 deno 的架构学到什么

陈天，陈天，目前是北美最大的免费流媒体服务TubiTV 的研发副总裁，曾创立在线旅游平台途客圈。著有《途客圈创业记》（人邮出版），《陈天·Rust 第一课》（极客时间出品）。公众号《程序人生》，知乎专栏《迷思》的作者。马拉松爱好者，两个女孩儿的父亲。工作十八年以来，一直从事高性能系统的研发工作，涵盖网络协议、网络安全、服务端架构、区块链以及云服务等方向。目前积极探索 Rust 在高并发网络生产环境中的使用。

介绍 deno 架构及其要解决的问题，并且了解为什么 deno 使用 Rust，从而给我们什么启示。

##  Rust助力量化高频交易

陆一洲，非凸科技量化策略负责人

本次演讲分享非凸科技如何利用 Rust 提高策略稳定性，大幅降低意外回撤率等相关实践。



##  使用 Rust 构建云原生数仓 Databend

尚卓燃，Datafuse Labs 数据库研发工程师，开源社区活跃贡献者。

内容简介：Databend 是一个使用 Rust 研发、开源、完全面向云架构的新式数仓。本次分享将会介绍「 Databend 的架构和设计」以及 「Databend 团队的 Rust 之旅」。





# 分会场 4: Rust 生产实践

## Rust ETL 和后端服务实现

讲师： 张文超 - 章鱼网络


重点介绍当前 Rust 微服务生态以及应用，占用资源优势以及高并发降低开发者心智负担的优势。以及介绍使用 Rust 编写 PostgreSQL 插件和 GraphQL 无服务器后端。结合 NEAR Indexer 项目介绍 ETL 方向 Rust 的应用以及优势。




## 高性能 Rust RPC 框架设计

徐帅，2017 年开始接触 rust, 有幸成为 rust team member, 一直致力于挖掘这门语言的潜力，并希望吸引更多的使用者, 同时壮大社区。现在在字节跳动基础架构团队探索 rust 在性能和安全问题上的更多可能性。

我们都知道 "机器比人便宜, 能加机器就加机器" 的这一道理, 在字节, 我们遇到了困境, 机房容量有限, 自建机房周期太长, 跨机房延时太高等等, 无法再去肆意挥霍机器, 也不能想加就加, 彻底打破了这一道理. 在存量优化的阶段, 我们希望有更好的技术选择, 就和当年大家在知道摩尔定律失效之后一样. 当然机器确实比人便宜:)

##   CeresDB 中的一种并发模型实践

讲师介绍： 夏锐航，蚂蚁集团资深技术专家

内容介绍：面对时间序列数据存储的需求，我们使用 Rust 构建了一个时序模型的 KV 存储引擎，在数据组织、异步 I/O 及 Thread Per Core 等方面进行了探索，并在本次 Talk 中向大家分享这一过程中的经验与体会。



# 分会场 5: 加密、隐私与可信计算

## 简看Rust密码系统生态和实现

王江桐：毕业于美国加州大学尔湾分校，就职于华为，目前正在使用Rust开发密码相关模块。密码学与Rust编程爱好者，正在学习并致力于分享有关Rust语言、生态以及密码学相关知识。

介绍Rust社区中密码学生态的现状，并结合当前项目密码算法和安全协议的开发实践，分享Rust在密码算法上的开发优势和经验。

## 基于Rust的分布式隐私计算实践

韦晓亚，在数牍科技主导高性能的分布式隐私计算框架的开发。加入数牍之前，他曾供职于Airbnb和Google Cloud，在分布式系统方面积累了丰富的经验。

数牍科技基于Rust语言针对隐私计算的特性研发了一套分布式的计算框架。我们将介绍隐私计算的特点，Rust语言的安全和高效特性如何帮助我们实现高性能的分布式计算，以及我们对于Rust语言的使用体会。

## Teaclave: 从可信执行环境基础到安全计算平台

孙茗珅，Teaclave PMC

在大数据时代，数据的开放共享、资源整合和安全保护已经成为重要的话题。传统数据处理方式已经无法满足现代数据的采集、流通、计算中对于安全的需求。隐私保护技术的出现正是为了解决这一问题，打破数据壁垒，解决数据孤岛困境。Rust 的内存安全保证、最小运行时、零成本抽象为隐私计算提供了安全可靠的开发基础。在这次演讲中，我们将了解隐私计算和可信执行环境的基本知识，为什么编程语言的选择对隐私计算系统开发如此重要。以 Apache Teaclave (incubating) 项目为例，介绍在项目实践中探索 Rust 在隐私计算应用的最佳编程实践。最后，我们将会了解在可信执行环境和隐私计算方向上，Rust 生态还需要补齐哪些方面，为未来的项目的发展提供思路。

## 在 Intel SGX环境下实现 Rust 原生 std 支持

周顺帆博士毕业于复旦大学系统软件与安全实验室，曾在国际顶级安全会议 USENIX Security 上发表对于以太坊生态中攻击交易与防御手段的研究，并协作发表多篇国际顶级安全会议论文。是《Phala Network 白皮书》的联名作者，并参与设计了 Phala 的系统架构。周博士负责带领Phala研究和工程团队在算法、系统架构、网络优化方面逐步提升 Phala 云计算的先进程度，在其带领下目前已在SGX里实现了phala-blockchain的密钥管理核心功能。

Intel SGX是一个把应用与OS完全隔离的可信执行环境，应用无法直接访问OS提供的资源。我们采用的Teaclave-SGX-SDK只提供了no_std环境，导致crates生态下大量的库都无法被使用。为了在SGX环境下开启std支持，我们通过补齐libc缺失的函数，实现了对OS基本功能的模拟。为了保证尽可能小的安全边界，我们对每个增补的libc函数做了权限控制。同时引入了二进制分析，确保程序不会出现SGX非法指令。



# 分会场6: 嵌入式、操作系统与物联网

## Rust for Linux is Coming

讲师：施继成，达坦科技联合创始人

简介：Rust for Linux 离进入 Linux 主分支已经不远了，大家准备好使用 Rust 开发 Linux 内核了吗？本次分享主要为大家介绍 Rust for Linux，并且带领大家写一个内核模块，从编写代码到编译上线，综合体会 Rust for Linux 的使用过程。最后也给大家带来一些 Rust for Linux 的编写经验和原理解释，帮助能够深入了解这一技术。

## 嵌入式Rust与RustSBI固件设计

洛佳，华中科技大学网络空间安全学院大四学生，4年Rust开发经验，热爱Rust嵌入式和操作系统开发工作。目前致力于向教学、研究和产业界推广使用Rust语言。

本次演讲，我们将从嵌入式Rust出发，描述产品可用的RISC-V固件应用例子。作为用途广泛的内存安全语言，Rust将在物联网、能源等领域大放异彩；厂商、社区如何参与嵌入式Rust的开发体系？固件软件保持在内核后台运行，事关RISC-V系统的安全、可靠，其稳定性不容闪失，该如何用Rust语言保证这一点？最后，我们将介绍RustSBI和Oreboot引导程序项目，这些优秀的项目诞生于RISC-V固件可移植和开放、易用性的呼声，是嵌入式Rust生态用于RISC-V SBI固件的良好示例。

## 协作式机器人和物联网的 Rust 实践

田劲锋，乐白科技工程师

介绍Rust在机器人控制器开发、运动控制、实时系统、物联网、WebAssembly的实践。



# 分会场 7: 分布式系统实践

## 基于 Rust 的下一代分布式存储 - HydroFS

宁安，前豆瓣网DBA, 目前任职青云, 文件存储和对象存储架构师

Hydrofs 是基于 rust 从0开发的一款支持 posix 语义的分布式存储, 此次演讲会阐述我们创新的设计哲学和分布式理论, 以及分享 Rust 在系统编程方面的独有优势

## Madsim：神奇的分布式系统确定性模拟器

Madsim: Magical Deterministic Simulator for Distributed Systems.

王润基，清华大学计算机系硕士生，Singularity Data 研发工程师。主要作品包括 Rust 操作系统内核 rCore/zCore 与高性能分布式文件系统 MadFS。

介绍

构建完全正确的分布式系统非常困难。如果你做过 6.824 的 Raft 实验，相信你一定遇到过那种运行上千次才蹦出一次的 bug 并因此调到怀疑人生。为了解决这一问题，我们用 Rust 开发了确定性的分布式系统模拟器 Madsim。基于 Madsim 的 Raft 实验，你可以在 1 分钟内将全部 50 组测试用例运行 100 次，并在出现问题后随时复现相同的执行过程，大幅提高开发调试效率。本次分享将介绍 Madsim 的实现原理，以及在实际项目中落地应用的经验。

大纲

* 分布式系统的特点和挑战
* 确定性模拟器 Madsim 的实现原理
* MadRaft 效果演示
* 在分布式文件系统和数据库项目中的落地经验



## 面向分布式服务架构的高可用流量控制组件 Sentinel 的 Rust 实现

杨培灏目前为上海交通大学在读硕士研究生，研究兴趣为物联网、云计算，在国际会议、期刊发表了多篇论文，曾获得杨元庆奖学金、博世 AIoT 奖学金等荣誉奖项。此次会议中，作为 Sentinel Commiter，分享阿里巴巴开源项目“面向分布式服务架构的高可用流量控制组件 Sentinel 的 Rust 实现”。

随着微服务的流行，服务和服务之间的稳定性变得越来越重要。Sentinel 是面向分布式服务架构的流量控制组件，主要以流量为切入点，从流量控制、熔断降级、系统自适应保护等多个维度来帮助您保障微服务的稳定性。Sentinel 拥有庞大的开源社区和众多的使用者，随着 Rust 生态在云原生领域的蓬勃发展，社区也开始尝试进行 Rust 版本的 Sentinel 开发。





## workshops



### 达坦科技 Workshop: 用Rust实现RDMA高性能编程

RDMA是常用于超算和高端存储领域的高性能网络协议。RDMA有专用硬件网卡用于协议解析，同时RDMA的数据通路实现内核旁路，这样在RDMA网卡收发数据包时，可以完全避免由内核处理数据包导致的额外内存拷贝以及上下文切换，因此RDMA在网络传输方面相比内核的TCP栈可以达到很高的性能。

但是用RDMA开发网络应用比基于内核的TCP栈要复杂很多。首先，由于RDMA的数据通路不经过内核，因此在用户应用要发送和接收数据时需要自行管理内存，特别是在接收数据时，用户应用必须保证收到的数据不能超过接收内存区域的大小，否则RDMA协议栈会报错。其次，由于RDMA的单边操作是完全由硬件处理没有软件参与，因此接收端的用户应用完全无法感知RDMA单边操作，使得接收端RDMA应用有可能在单边操作执行的过程中修改内存，导致单边操作传输的数据出错，更严重的是接收端和发送端都无法感知数据出错。再者，RDMA的API是基于C实现，非常底层，需要用户在开发时要格外注意，不然那就会导致出错，比如RDMA用于接收和发送数据的内存区域必须是在堆上分配，不能是在栈上分配。

针对RDMA开发的种种不便，我们用Rust封装了一套RDMA的API，一方面简化RDMA开发的复杂度，另一方面保证用户应用实现高性能收发RDMA数据包，不会因为采用Rust封装RDMA的API导致有额外的性能开销。

本次Workshop准备了动手实验环节，方便大家实际体验如何用Rust构建RDMA应用，建议大家提前准备好实验环境。本次Workshop的相关资料，包括实验环境准备、动手实验的代码等，参见https://github.com/datenlord/Rust2022Workshop

欢迎对RDMA感兴趣的朋友参加本次Workshop！

**报名方式**：加入 Zoom 会议

https://us06web.zoom.us/j/81327298846?pwd=aWh1LzBaL2ZMakI3WFc3amVjekxPQT09

会议号：813 2729 8846

密码：0731





### 章鱼网络 workshop : 通过Substrate-Ibc实现Substrate资产跨链

主讲：苏胤榕，章鱼网络工程师

RustChinaConf 2021~2022大会 7.31 下午 16:00 章鱼网络 WorkShop 腾讯会议房间号：314-147-965

Substrate-IBC是由Interchain基金会资助， 由章鱼网络提出并开发的一个提案。Substrate IBC 模块，也称为 pallets，是连接Polkadot和Kusama与Cosmos链的重要一步，使两个生态系统之间的资产和数据的安全交换成为可能。Substrate-IBC 模块，将使开发者能够创建他们自己的具有IBC功能的Substrate区块链。 这个模块的目标是让建立在Substrate上的区块链可以通过IBC协议以无信任方式与其他支持IBC的区块链链交互。



###  Near Protocol Workshop | Rust 智能合约开发：从入门到精通



**介绍**：Rust 由于其高效、安全的特点，被广泛应用于区块链技术中，其中也不乏通过 Rust 开发智能合约的探索。

作为新一代高性能区块链，在 NEAR 上，使用 Rust 开发智能合约具有出色的开发体验、运行效率和安全性。

本次讲座中，NEAR 工程师 Daniel 将介绍使用 Rust 开发智能合约的入门方法和学习路径，并分享实战中的挑战与心得，帮助有兴趣使用 Rust 开发智能合约的开发者循序渐进，成为合格的 Rust 合约工程师。

**参考资料**：

- NEAR 开发者文档：https://docs.near.org/ 
- NEAR 中文社区学习视频：https://space.bilibili.com/492846343 

**时间**：7月31日下午4点~6点

https://meeting.tencent.com/dm/spbmQ9eD0yeW

腾讯会议：792-549-948

###  wasmedge Workshop **《Low Code Rust！使用 Rust 解决 SaaS 定制化问题》**

**介绍**：SaaS 已经全面“入侵”我们的生活与工作。我们通常面临着定制 SaaS 来满足个人使用的需求，因此 SaaS 公司一般提供了 API ，供开发者来定制 SaaS，实现千人千面的需求。相较于开发者自己起一个服务器的方式，通过 Serverless 的形式定制 SaaS ，对开发者是一个省时省力省钱的选择。

在这场 workshop ，Second State 研发工程师 DarumaDocker 将以 GitHub 为例，演示如何使用 Rust 函数与 Wasm 解决 SaaS 定制问题。通过这场 workshop，你也根据自己定制 SaaS 的需求编写 Rust 函数。



**时间**：7月31日下午4点~6点

会议号：300 735 578

https://meeting.tencent.com/dw/86R5nx9iKGI5