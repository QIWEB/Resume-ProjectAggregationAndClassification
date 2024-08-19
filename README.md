# Resume-ProjectAggregationAndClassification
简历-项目介绍个人职责业绩，技术说明，主要是it相关开发简历，运维测试前端java c vue等

==============2024年8月19日 ==========
项目经历
即刻享动 java后端开发 2023.06-至今
项目介绍：即刻享动是一款面向运动用户分享运动记录和经验并提供一系列教程视频等的综合交流社区。项目采用前后端分离开发，
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
2. 历史月榜表优化：后续考虑到海量数据的存储数据库问题，选择对月榜数据根据月份进行分表，减轻了数据库单表压力过大。 聆听妙音 java后端开发 2022.11-2023.06
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
誉美医院预约体检 java后端开发 2021.09-2022.11
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