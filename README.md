# Resume-ProjectAggregationAndClassification
简历-项目介绍个人职责业绩，技术说明，主要是it相关开发简历，运维测试前端java c vue等

==============2024年8月19日 ==========
项目经历

## 项目名称：IDS 数据迁移服务+IDS 后台管理系统 项目时间：2023.10-至今
项目描述：
IDS 作为太平洋保险内部系统间数据交互的核心枢纽，承担着数据传输与整合的关键任务。通过
应用阿里 DataWorks 等技术，构建了一个数据处理流程。该流程不仅能够高效地执行数据清洗和去
重任务，确保数据的准确性，还通过数据管理策略，保障了数据在传输过程中的完整性和一致性。使
用 Java 接口确保了业务流程的功能完整性，实现了数据处理的无缝对接和高效率执行。此外，IDS
后台管理系统提供了一个全面的管理平台，它对 Java 接口使用的配置进行了精细管理，并对管理端
用户的权限进行了限制，从而增强了系统的安全性。系统还具备对数据传输结果的实时监控功能，确
保了数据处理的透明度和可追溯性。
使用技术：阿里 DataWorks+MaxCompute+SpringBoot+MyBatis+OceanBase
项目职责：
1.参与项目的前期准备和初步开发研讨，参与业务需求设计。
2.进行 DataWorks 数据处理流程的设计与实现。
3.数据服务 Java 端接口的设计与实现。
4.进行管理端登录以及角色权限管理功能的的设计与实现。
5.跟进项目上线。

## 项目名称：太平洋庆亚运活动 项目时间：2023.07-2023.10
项目描述：
在亚运会期间，太平洋寿险通过其公众号平台推出了一项创新的营销活动，旨在提升品牌知名度
并吸引潜在客户。该活动精心设计了主会场和多个特色分会场，包括乒乓球和 AR 篮球等互动环节，
为用户提供了丰富的参与体验。
用户在各个分会场参与游戏，通过竞技和互动获得排名，并根据排名赢取奖品。此外，主会场还
设有签到任务，用户完成签到后可以观看视频和海报，从而获得额外的抽奖次数。抽奖环节为用户带
来了更多的惊喜和奖励，进一步增强了活动的吸引力。
使用技术：SpringBoot+MyBatis+MySQL+Redis+XXL-JOB
项目职责：
1.参与活动的业务规划和设计。
2.负责后端接口的开发。
3.跟进上线与后续提数。

## 项目名称：E 行销 项目时间：2023.03-2023.06
项目描述：
E 行销是一个创新的营销平台，专为业务员设计，以提高他们的市场推广效率和客户获取能力。
该平台利用微信这一广泛使用的社交平台，允许业务员轻松分享产品信息、创意海报和促销活动，从
而吸引潜在客户的注意力并促进销售转化。该项目分为管理端和移动端，管理端是后台操作的中枢，
允许管理员精心配置和定制各类营销素材，确保内容的多样性和针对性。而移动端则是使业务员能够
随时随地访问和分享营销资料，实现业务推广的即时性和个性化。
使用技术：SpringBoot+MyBatis+OceanBase+Redis
项目职责：
1.根据需求参与功能和设计。
2.负责移动端微信登录、积分任务、积分兑换等功能开发。
3.参与管理端登录、角色权限控制等功能开发。


## 2019-01 ~ 至今 2 翼支付客户端附近 翼 开发开
项目简介 项 ：该项目用于根据翼支付APP用户的实时定位，查询并展示附近的商户和该用户可参与的营销活动。
职责描述 职 ：
1.需求分析、设计以及数据库表设计和流程图的输出
2.进行核心功能的开发，包括首页商户检索展示。
3.根据性能测试结果进行系统性能优化
技术描述 技 ：
1.系统之间采用dubbo调用
2.用elastic-search进行商户检索
3.多线程异步调用查询商户活动，通过Future获取调用结果
4.使用redis对部分数据进行缓存，减少和DB的交互
5.使用自定义注解进行权限的校验
## 2017-10 ~ 2018-06 2 电信翼支付收单系统 电 开发开
项目简介 项 ：
“我的店铺”平台为商家和用户提供统一的收单解决方案。在这个平台上，商户可以自主决定是否给消费者提供
打折模式。为商家开放支付，订单详情查询和退款等功能
职责描述 职 ：
 项目经验
83e7d33fe22fecd51nVy2Ni1F1FYy422VfyWWOainfXVNhJh
83e7d33fe22fecd51nVy2Ni1F1FYy422VfyWWOainfXVNhJh
2017-05 ~ 2017-09 2 电信翼支付订单消息通知系统 电 开发开
1. 参与项目接口文档的编写，利用visio和Astah画出流程图和时序图。
2. 进行收单流程的优化和商户查询订单模块的代码编写。
3. 配合测试人员对项目进行接口测试和流程测试。
   技术描述 技 ：
1. 项目中采用SSM框架，降低各层之间的耦合度，数据库采用Oracle
2. 使用dubbo实现项目的分布式操作
3. 各系统之间的消息通知采用kafka消息中间件，使用多线程处理消息任务，提升系统的速率。
4. 用redis对部分数据进行缓存以减少服务器跟数据库的请求压力。
   项目收获：
   这段工作经历让我对第三方支付业务有了一个整体的认识，并且学习使用了大量插件跟中间件，提升了自我的学
   习能力，通过大型项目的开发加强了本人的团队协作能力以及多部门协同开发时对工作的推进能力
## 2017-05 ~ 2017-09 2 电信翼支付订单消息通知系统 电 开发开
项目简介：本项目对接收单产品，为每个商户进行订单状态的通知，通知类型包括http回调，短信发送，消息推送
等。
职责描述 职 ：
1. 配置表的设计和开发。
2. 使用junit进行单元测试。
   技术描述 技 ：
1. 项目中采用SSM框架，数据库采用Oracle。
2. 使用dubbo实现项目的分布式操作
3. 使用guava异步处理发送消息提高效率和guava的异步回调提高性能。
4. 用redis对部分数据进行缓存以减少服务器跟数据库的请求压力。
5. 将要发送的消息放入redis队列，使用@PostConstruct启动后台线程从redis队列读取消息内容进行任务处理。

## 即刻享动 java后端开发 2023.06-至今
- ** 项目介绍：**
  即刻享动是一款面向运动用户分享运动记录和经验并提供一系列教程视频等的综合交流社区。项目采用前后端分离开发，
有App端及后台管理端两个平台。在该应用中，用户可以在运动达人榜中进行比拼，发布文字、视频作品分享自己对运动的经验，在
社区模块中观看视频学习。后台管理端要对用户发布内容进行审核和标签化分类，敏感词管理等。
技术栈：SpringBoot、SpringCloud、MySQL、MyBatis-Plus、Redis、GateWay、Nacos、OpenFegin、Seata、Redisson、
Docker、XXL-Job、RabbitMQ、Jenkins。
个人职责：
1. 教学视频模块：
(1) 用户视频上传：使用了腾讯云的VOD视频点播上传视频，用户可以在首页的加号处点击发布作品后选择上传视频到服务端。
(2) 视频审核：服务端接收请求后对接第三方智能检测视频内容，检测异常的后由人工审核。
0bc71679cb812c171nVy2Nm-FVtSw4-5VvqaWO2hn_LSMRNr
(3) 视频上架：审核通过后服务端初始化VOD客户端并上传至VOD平台生成唯一标识field。后续的删除、隐藏视频就根据field来
定位视频并修改状态。采用POST请求接收平台回调视频信息并持久化。
(4) 后台视频分类：使用Caffeine的高性能作为本地缓存库，加快访问速度,减少网络带宽的消耗。
(5) 实现教学视频的维护：用户可以收藏自己喜欢的教程到收藏夹，免费的教程可添加成功，付费的则需要支付后才可添加。
(6) 视频的续播：采用延迟任务进行合并写实现用户观看视频直接关闭客户端或切换设备做到20S误差以内的续播。
2. 活力值模块：
(1) 签到功能：使用Redis中的BitMap来保存签到记录，使用BitField命令获取签到记录。
(2) 活力值：活力值由签到、观看教学视频、评论等组成，为了防止各服务之间的高耦合，采用MQ异步方式。
(3) 运动达人榜：分为了当前榜和历史榜，历史榜采用XXL-Job每月初3点更新前一个月的活力值月榜单到数据库。
3. 评论模块：
(1) 用户评论回答：用户可以在其他用户分享的文字、视频作品下评论，并且可以进行回复。
(2) 评论举报：用户可以对不良言论长按后选择举报评论。
(3) 用户禁言解禁：发送HTTP请求调用阿里云文本审核API，接收审核返回结果如达到禁言标准，修改用户评论状态禁言后使用
XXL-Job设置定时任务根据封禁时段解禁该用户评论。
(4) Redis 点赞记录：通过 Set 集合来记录用户点赞限制，避免用户重复点赞。
(5) 点赞总数统计：采用了合并写方案减轻高并发写对数据库的压力，定时任务定期发送MQ同步业务点赞总数。
业绩:
1. 实现视频续播高并发优化的方案：前端会每15秒发送一次请求记录播放信息，改用Redis的hash来缓存信息，通过 RabittMQ
发送延迟消息确认从而合并数据库写请求，缓解数据库压力，极大的降低响应时间，将延迟时间设置为20秒，然后比较Redis中的播放
记录时间戳与MQ消息中的是否相等，相等说明用户15秒内没有观看视频，接着数据持久化到数据库并清空Redis缓存。
2. 历史月榜表优化：后续考虑到海量数据的存储数据库问题，选择对月榜数据根据月份进行分表，减轻了数据库单表压力过大。
##  聆听妙音 java后端开发 2022.11-2023.06
项目介绍：聆听妙音是一个基础SpringCloud微服务架构开发的轻音乐App系统，用户可以在应用内搜索不同种类的音乐类型进行收
听，还可以通过应用内的限时减免卡券购买专属特权，用户端的核心业务有：音乐搜索、购买特权、收藏音乐、评论点赞等；管理端
的核心业务有：用户管理、音乐上传维护、营销活动推送等。
技术栈：SpringBoot、SpringCloud、MySQL、MyBatisPlus、Redis、ElasticSearch、GateWay、Nacos、OpenFegin、Seata、
Redisson、Docker、XXL-Job、RabbitMQ、Jenkins。
个人职责：
1. 限时减免模块：
(1) 优惠券发放：分为定时发放和立即发放以及手动领取和兑换码兑换，采用XXL-Job实现定时发放限时优惠券。
(2) 优惠券的领取：面对高并发场景，存在超卖问题，采用分布式锁 Redisson解决。
(3) 优惠券的兑换码算法：借鉴 JWT 令牌思想，通过自增 id、密钥加权，随机数等一系列算法通过 Bese32转码得到。
2. 查询模块：
(1) 歌曲搜索：该模块使用ElasticSearch完成音乐的检索。采用Canal完成数据同步。
(2) 热门推荐：根据用户收藏音乐的标签推荐音乐，关联数据有用户收藏音乐数据和绑定的音乐标签属性。
(3) 分类筛选：建立歌曲与分类中间表联系，根据分类ID筛选出歌曲。
3. 用户模块：
(1) 收藏歌曲：用户可以将喜欢的歌曲收藏到收藏夹进行管理。
(2) 历史播放记录：播放一首歌曲时添加到历史记录，对历史记录进行时间排序显示最近播放的歌曲。
(3) 优惠券管理：在调用支付服务时使用优惠券，用户可在管理中知悉自己的优惠券信息。点击使用跳转至优惠券限定的使用方
位服务中。
(4) 偏好设置：该页面展示歌曲分类，根据喜好添加音乐分类将User表中interesting_categroy字段添加分类ID。
4. 自动化部署：使用Jenkins+Docker搭配git私服,完成项目在开发和测试环境下的自动部署。
业绩:
1. 发放优惠券兑换码优化：单个优惠券生成1000个兑换码会产生高并发写DB，测完延迟在将近3S，后续采用SpringBoot异步开
多线程写来提高性能，优化后接口速度在几十毫秒。
## 誉美医院预约体检 java后端开发 2021.09-2022.11
项目介绍：誉美医院预约体检，是向C端用户提供体检服务的系统。旨在提供方便、快捷、安全的体检预约服务，让用户能够随时随地
预约体检，并获得相关的健康咨询和服务。通过小程序，用户可以随时了解自己的身体健康状况，及时发现和预防潜在的 健康问题，
同时也可以获得权威的健康资讯和建议，更好地管理和维护自己的健康。
技术栈：SpringBoot、SpirngMVC、MyBatis-Plus、MySQL，Redis、Spring Task、HttpClient
个人职责：
1. 预约模块：
(1) 预约订单处理：用户预约体检时间段成功后，订单处于待完成，超出预约时间后用户未到达需要将订单状态置为已过期，采
用了Spring Task定时任务定期查出超出预约时间的订单，修改订单状态。
(2) 预约体检：在小程序首页点击预约体检后，用户可以选择预约的类型、时间段进行预约体检。由于预约功能是系统的高频接
口，选择了Redis进行存储订单数据，定时任务每天把已完成或已过期的订单进行数据库持久化。
2. 小程序登录模块：
(1) 微信小程序登录：用户在小程序端可选择游客访问，但是点击预约等功能就需要登录才能访问，用户同意手机号授权登录
后，会调用wx.login携带code，nickename，detail.code发送请求给服务端，服务端接收后携带appId+appsecret+code
三个参数通过HttpClient向微信平台接口发送请求，返回openid，根据用户信息生成jwt令牌，然后返回token信息给前
端，后续用户在操作需要身份校验的功能时候都会携带着token中的信息去访问。
(2) 用户APP验证码登录：随机生成五位验证码并存入Redis里设置超时时间，使用第三方服务阿里云短信服务进行向用 户手机
号发送短信。
3. 后台登陆模块：
(1) 后台登录鉴权：后台登陆时，拦截器排除登录接口，对账号密码进行校验，获取用户所拥有的权限（基于RBAC角色模
型），将资源权限存入Redis并根据用户信息用jwt封装token。后续访问携带token数据，对于拦截器未排除路径的请求进
行拦截鉴权，Redis资源和请求资源进行match成功后将用户信息Set进ThreadLocal。
(2) 后台验证码登录：使用字节数据输出随机生成四位字母＋数字存入Redis里并设置超时时间，登陆时进行验证中；
4. 公共字段填充：
根据自定义注解标识需要增强的方法,自定义注解里面增加枚举类属性细分增强类型,使用AOP切面类进行统一拦 截,将一些重
复性代码抽象出来,进行集中处理,减少代码冗余。


## 项目 1：上交所新期权风控系统
开发环境： idea+jdk1.8+git+ Jenkins+VastBase+ AnalyticDB PostgreSQL+redis+rabbitMq
软件架构：springboot 框架
开发时间：2022.8 –-至今 开发周期： 23 个月
项目描述： 上交所新期权风控系统是上交所对期权交易的风险监控和监察，对老期权风控系统框架升级和
国产数据库替换改造，提高系统整体性能，提高业务人员对期权交易数据实时监控分析，预警期权风险及
时处置，提高业务人员工作效率；主要模块包括首页，预警中心、风险分析、风险处置、风险展示、监管
知识库、基金、科创板、沪伦通做市、系统管理等。
责任描述：
1. 参与项目需求分析，详细设计文档编写，负责业务需求功能代码实现；
基本信息：
教育背景：
求职意向：
开发技能：
工作经历：
a20d2f1b627a074f1nVy2Nm8ElNSwYS-UPKbWO2hn_LSMRNr
a20d2f1b627a074f1nVy2Nm8ElNSwYS-UPKbWO2hn_LSMRNr
2. 编写详细设计文档并参与代码评审，代码重构，sql 优化，配合前端联调和 JIRA 问题单修复；
3. 线上问题查找原因和提供解决方案；
## 项目 2：支付结算人民币系统
开发环境： Eclipse +jdk1.7+git+ Jenkins+Oracle
软件架构：SM 框架
开发时间：2020.9 –- 2022.8 开发周期： 24 个月
项目描述： 建行支付结算人民币项是人民币二代支付系统，对不同的交易渠道发起大额、小额、网银交易
等业务处理的核心中间组件，对客户交易服务安全的重要保障，交易数据准确性验证，清分出支付资源，
根据支付资源，记账场景试算出需要记账的内部账号，调用相关的主机交易服务记账，记录交易信息，交
易状态信息，交易记账信息，保证交易一致性。
责任描述：
1. 参与项目需求分析，负责迭代业务功能需求代码实现和前端交易页面开发；
2.负责生产 DCM 单事件处理；
3.配合测试修复 bug，后期的功能优化，模块代码重构；
4.编写功能说明文档。
## 项目 3：建融智合服务平台 链接：https://want.ccb.com/essp/#/userIndex/login
开发环境： idea+jdk1.8+svn+yunSO+Oracle
软件架构： Springcloud 微服务框架
开发时间： 2020.4–- 2020.8 开发周期： 5 个月
项目描述： 建行企业智能撮合共享服务平台集智能撮合、企业中心、需求大厅、咨询大厅、智慧生态圈 , 精准扶贫，个人中心、用户服务、消息中心、代办事项等为一体的综合服务平台；为了实现帮助企业打造
企业圈，构建智慧园区，展现实力的舞台，服务上架自助营销 ,需求快速发布，连接供需两方，大数据智
能匹配，贴心线下撮合服务平台。
责任描述：
1.参与项目需求分析包括用户服务、企业橱窗服务、企业商品管理服务；
2.负责后台公共用户服务和企业橱窗服务的功能代码实现和前端接口的对接；
3.配合测试修复 bug，后期的功能优化，模块代码重构；
4.参与部分功能说明文档的编写。
技术描述：
使用 poi 实现白名单的模板下载和数据导入； 使用 SpringCloud 实现企业橱窗模块，用户模块 WEB
服务，Feign 服务接口开发，和 redis 同步缓存，使用 Mybatis 分页插件 pagehelper 实现分页等。
## 项目 4：零售分池和组合风险后台报表开发
开发环境： Cognos +Oracle
开发时间：2019.2 –- 2020.3 开发周期： 13 个月
项目描述：中国建设银行企业零售分池（RECRM）和组合风险（PRMS）报表系统更新（180 多张报表）， a20d2f1b627a074f1nVy2Nm8ElNSwYS-UPKbWO2hn_LSMRNr
数据库变更（TD 数据库迁移 Oracle 数据库）及新需求的前台报表开发（Cognos10），更好的为总行和一
级分行客户提供报表服务和业务智能解决方案。
责任描述：
1.负责零售分池和组合风险项目报表迁移及部分新增报表需求分析，数据库表设计；
2.负责报表工作计划安排，后端报表模型创建，数据项开发，报表页面和提示页开发；
3.配合测试人员修复 bug，和报表性能优化(Sql 性能优化)；
4.报表维护文档和报表功能文档说明的编写。
## 项目 5：上海银行 ITM 管理平台
开发环境： idea+jdk1.7+svn++tomcat7+Oracle
软件架构：SSM 框架
开发时间：2017.2 –- 2019.1 开发周期： 23 个月
项目描述：上海银行 ITM 是将银行网点的业务办办理，更加专业化，智能化，提高用户的业务办理效率，
使线上与线下资源更有效整合，全面优化业办理服务平台；ITM 管理平台分为 ITMC(机具端)，ITMP（现金
P 端）和 ITMM（管理 M 端），后端管理模块包括：公共管理，设备管理，版本管理，监控管理，业务报
表，设备报表等。
责任描述：
1.参与项目需求分析包括角色权限按钮的细化，公共管理模块卡品种下发，版本模块中版本下发、营
销图片下发，业务报表模块中的业务报表统计，历史明细查询，设备报表模块中机具完好率，机具开
机率；
2.负责后台业务功能需求代码实现和前端页面编写；
3.配合测试修复 bug，后期的功能优化，模块代码重构；
4. 编写功能说明文档。
技术描述：
使用自定义线程池实现管理平台到机具端卡片，营销图片，版本的下发；使用 poi 实现业务报表功能
导出；使用 spring 定时器实现历史明细数据的管理。


## 项目一：选象saas
项目描述：
选象saas：选象平台进行商品的的上下架及平台的一些轮播图的小程序端展示设置，小程序：不同品牌的
门店可以在小程序下单，启动设备，公告，轮播图等。项目采用SpringCloud微服务架构，其中包含用户中心，
商品中心，交易中心，支付结算中心，消息中心，客服中心
责任描述：负责老商品的技术迭代，参与新商品系统重构，抽象SPU，SKU等相数据关模型，以及编辑商品，商
品搜索，商品上架等核心模块代码开发
基础架构支持：公司日常util组件开发，比如异步导出，日志组件等
## 项目二：工单系统
项目描述：
项 目 是 隶 属 于 选象系统 的工单系统、第一版对接合力亿捷 ，存在同步失败的情况，通过定时任务扫描
失败的工单重新提交，第二版实现完全自研，实现自定义的一些功能，小程序：不同品牌的门店可以在小程序
对设备进行报修，维修人员可以在小程序进行相关节点的变更，项目采用SpringCloud微服务架构，数据库采用
mysql 数据库
责任描述：在项目中主要负责表结构设计，设备报修等核心代码开发以及需求迭代开发
## 项目三：溯源绑定系统
项目描述：
项 目是隶属 于选象系统的溯源绑定系统、该系统主要对于货物的跟踪，防止发生串货现象，原先通过小程序进
行绑定，后续对接外部系统，采用RFID标签实现发货自动绑定， 通过定时任务进行前一天数据的同步，通过
RabbitMq通知物联网，完成数据校验及数据同步，项目采用SpringCloud微服务架构
责任描述：溯源表结构设计，溯源绑定等核心功能开发
## 项目四：溯源码系统
项目描述：
项 目 是 隶 属 于 选象系统 的溯源码系统迭代、 根据各商品生成自定义条码，原先是打印粘在外包装，后续迭
代成RFID，更方便进行发货绑定及物流溯源，项目采用SpringCloud微服务架构
责任描述：溯源码迭代表重新设计,历史数据同步，码规则设计，码生成等核心代码编写及后续迭代
## 项目五：服务卡系统
项目描述： 02783df686d42d2f1nVy2Nq_FFRXyoy5U_-aWO2hn_LSMRNr
项 目是隶属 于选象系统的服务卡系统、服务卡系统便于门店根据各商品设置各种类型服务卡，便于门店去预售
一些新商品及管理门店会员， 各 系 统 间 调 用 使 用nacos实现高可用，接口幂等 : 主要使用 Redis 锁实现，数据
库采用mysql数据库
责任描述：表设计,服务卡购买、使用等核心开发及后续需求迭代
## 项目六：问卷系统
项目描述：
项 目是隶属 于选象系统 的问卷系统、自研的问卷可以做一些自定义的功能，便于统计及保护公司敏感信息安全，
各系统 间调用使用nacos实现高可用，接口幂等 : 主要使用 Redis 锁实现，数据库采用mysql数据库
责任描述：表设计,创建问卷、提交问卷等核心功能开发及后续需求迭代
## 项目七：SAP
项目描述：
项 目是隶属于 选象系统的SAP系统、各系统 间调用使用nacos实现高可用，接口幂等 : 主要使用 Redis 锁
实现，数据库采用mysql数据库，因公司战略调整开发完成未进行调试
责任描述：接口的对接及功能开发
## 项目八：交付履约
项目描述：
项 目 是 隶 属 于 选象系统 交付履约、 各 系 统 间 调 用 使 用nacos实现高可用，接口幂等 : 主要使用 Redis 锁
实现，数据库采用mysql数据库,因公司战略调整开发完成未进行调试
责任描述：数据表的设计开发
## 项目九：车 险项 目
项目描述：
项 目是隶属于 安盛天平 的 车 险项 目 ， 统一鉴权 中心 使用 Gateway 网关实现 、各系统 间调用使 用
Dubbo+zookeeper 来实现并通过搭建 Zookeeper 集群来实现系统的高可用，缓存 : 主要使用 Redis 实现, 用以
保存相同数据的请求直接从缓存读取，定时任务调RabbitMq做保单报价等数据的同步，数据库采用plsql和 orcal
数据库
责任描述：在项目中主要负责保费等核心模块的优化， 项目模块的新增，如新增 113 险种及付费模块的添加
等，批改等相关功能的优化及与其他系统的联调以及日常 bug 修复。