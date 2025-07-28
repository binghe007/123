# 冰河网络安全课程(2025)

### 第一期——web架构与搭建

##### 一. 首先想要了解web的架构并实践搭建

我们需要了解web的组成为:域名，主机/服务器，源码，ssl证书(了解即可)

###### （1）域名

![85fd33ff-70a9-4e74-a656-dba02ac7ca8c](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.1.png)

这个叫做域名

【域名的细分】域名分为一级域名，二级域名，三级域名......其中一级域名又称顶级域名

一级域名：<img src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.2.png" title="" alt="51dd0b17-6259-4709-b1b5-4c42db36654e" data-align="left">

二级域名：<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.3.png" alt="49618a57-70ae-4b83-99b9-bbad2480447a" data-align="left">

三级域名：<img src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.4.png" title="" alt="f1f63e25-b9e8-400b-a9ec-1d727f393c1e" data-align="left">

以此类推

###### (2)云主机(虚拟主机)/云服务器

市面上大厂的[idc商]([IDC服务商_百度百科](https://baike.baidu.com/item/IDC%E6%9C%8D%E5%8A%A1%E5%95%86/837458))都比较贵 如果是我们学习网络安全使用 或者是新手站长试水 完全没有必要花大价钱去买大厂的机器 哔哩哔哩上有很多跑路云供大家使用

【[云主机]([云主机_百度百科](https://baike.baidu.com/item/%E4%BA%91%E4%B8%BB%E6%9C%BA?fromModule=lemma_search-box))与[云服务器]([云服务器_百度百科](https://baike.baidu.com/item/%E4%BA%91%E6%9C%8D%E5%8A%A1%E5%99%A8?fromModule=lemma_search-box))的区别】购买云服务器相当于购买了一个可以远程链接的带有公网IP的电脑<mark> 一个云服务器可以分成多个云主机</mark> 用这个电脑进行建站而云主机只是给你一个虚拟空间 只能建站使用 总的来说云主机没有那么大的自由度 操作没有那么灵活 但价格也更便宜 推荐<mark>不想花太多钱的购买主机</mark> <mark>想深入了解建站细节的购买服务器</mark>  购买服务器对后期学习[渗透]([渗透（IT术语）_百度百科](https://baike.baidu.com/item/%E6%B8%97%E9%80%8F/9457427?fromModule=lemma_search-box))帮助更大 当然主机也是一样的 

小厂主机平均最低价格：0.1元/月     小厂服务器平均最低价格：16元/月

当然这么低价格的IDC商需要耐心寻找

推荐：[yun.timeidc.cn](yun.timeidc.cn)    2025.7.28可以薅0.1主机羊毛

##### <mark>***提示：所有机器国内的需要备案才能使用 国外以及港澳台的机器无需备案***</mark>

<mark>提问</mark>： 云服务器相当于用电脑搭建网站那我为什么不用自己的电脑搭建网站？

<mark>答</mark>：

个人电脑：需24小时开机，硬件损耗大（如硬盘、电源易损坏），且家庭网络易受停电、断网等影响，故障恢复完全依赖用户技术能力，可能导致长时间宕机。

个人电脑：家庭网络上传带宽有限（通常仅10-100Mbps），多人访问时易拥堵，且硬件升级成本高、周期长。

个人电脑：暴露公网IP后易受攻击（如DDoS、SQL注入），需自行配置防火墙和定期更新补丁，安全风险较高。

云服务器：自带独立公网IP，无需内网穿透（如cpolar工具），避免复杂配置和额外费用。

###### (3)源码

**源码就是预制网站你按说明部署就能快速建站，如果想完全自定义，也可以自己写代码（适合程序员)**

源码的分类：

| 类型    | 适合谁用     | 例子                   | 特点          |
| ----- | -------- | -------------------- |:----------- |
| 静态源码  | 个人简历、作品集 | HTML+CSS模板           | 简单、便宜，但功能少  |
| 动态源码  | 博客、论坛    | WordPress（PHP+MySQL） | 支持评论、用户管理   |
| 商城源码  | 开网店      | Shopify（付费）          | 含支付、购物车功能   |
| CMS源码 | 企业官网     | PageAdmin（后台管理方便）    | 非技术人员也能更新内容 |

源码建议上[GitHub](github.com)找进不去的话请用魔法上网

###### (4)ssl证书

有证书网站：

![18de2d5b-a378-4b6c-99ad-c64d6684d68c](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.6.png)

锁头显示安全 http<mark>s</mark>

无证书网址：

![c0fbea84-5f13-4db3-b19a-6f6f099ab3ec](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.7.png)

显示不安全 http

ssl证书也有免费的

##### 二. 实操

现在教你实操搭建一个网站

1.[购物车 | Little Time Yun](https://yun.timeidc.cn/cart?fid=18)先来买个服务器或者主机 这里用主机演示 服务器同理 但是要自己搭建管理面板服务器搭建教程https://zhuanlan.zhihu.com/p/423724615

<img src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.8.png" title="" alt="d676e475-d1f9-4611-9137-561dbef957ba" style="zoom:33%;">

再买个二级域名 免费的   [域名购买地址](https://dns.vdvz.net/user/#/shop/index) 这里选一个自己最喜欢的

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.9.png" alt="8bc28137-1a4b-4d8e-996f-a4aa18138b38" style="zoom:33%;">

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.10.png" alt="97659609-2102-46a6-be0e-eed85a2f2ff1" style="zoom:50%;">

![e29267bfa5a6b24b17e2ffca747de9be](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.11.png)

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.12.png" alt="581aec2f3e973f33c83395219a9f91c2" style="zoom:50%;">这是IDC商那里![2377cdb02e0c54d935ed811c42e65028](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.13.png)

再随便下载个源码 这里聊天室为例

https://github.com/jackyoung01/open-chatroom

<img src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.14.png" title="" alt="e493c691-2fa0-4fc1-ae6c-16bbed34a7ba" style="zoom:33%;">

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.15.png" alt="9036e8ca-bfa5-4a9b-a6e6-149fb92da008" style="zoom:67%;">

下载后拖到桌面

然后看一眼作者要求(最下面)

![2194cbdb-95fd-4a66-8bf5-2e2de8b747df](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.16.png)

然后回到IDC商

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.17.png" alt="屏幕截图 2025-07-28 173544" data-align="left" style="zoom:50%;">

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.5and1.18.png" alt="屏幕截图 2025-07-28 175448" style="zoom:50%;">

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.19.png" alt="41140029-2724-42f7-b759-3f90b48824ff" style="zoom:67%;">

![79b7a4e4a2667c85c1680dc02f55e66d](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/1.20.png)

![761ed72cbd75018343817ddacb1ac615](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/761ed72cbd75018343817ddacb1ac615.png)

![9246cdf51ea051cc09754f66898c969f](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/9246cdf51ea051cc09754f66898c969f.png)

![7a4669af7dfff9ad5ea0f2211ac714da](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/7a4669af7dfff9ad5ea0f2211ac714da.png)



![11e19bad-e833-41ac-9615-6b1fd78875d8](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/11e19bad-e833-41ac-9615-6b1fd78875d8.png)

这是域名商那里

<img src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/67f6c9c2e4c7d6db855752b27f06ffeb.png" title="" alt="67f6c9c2e4c7d6db855752b27f06ffeb" style="zoom:50%;">

然后点确认添加

现在域名绑定好了 源码也导入完了 但是作者给的说明要求手动配置数据库连接 以及将作者设计好的，现成的数据及数据库架构(.sql文件)导入数据库

但是作者有两点没说 

<mark>1.php版本要求7.4</mark><img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/007ab3dc7a55d25132c172e06a97597a.png" alt="007ab3dc7a55d25132c172e06a97597a" style="zoom:80%;">

2.后台管理系统密码作者没说 需要自己到数据库里找到admin表 手动修改密码 需要注意密码需要使用md5加密存在数据库中 后面再讲。

现在手动配置数据库连接

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/2c851e9c456cd80089d74eb62bed0ff9.png" alt="2c851e9c456cd80089d74eb62bed0ff9" style="zoom:67%;">

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/b7ac132718785e30eef5d81dabd15968.png" alt="b7ac132718785e30eef5d81dabd15968" style="zoom:50%;">

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/c4991d87c72006e3e8070b0293107de9.png" alt="c4991d87c72006e3e8070b0293107de9" style="zoom:67%;">

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/bf639f2f50a3347671fd3e5fd95ea70e.png" alt="bf639f2f50a3347671fd3e5fd95ea70e" style="zoom:67%;">

到这里数据库连接配置就配置好了 接下来进入数据库导入作者放在压缩包的.sql文件

回到电脑桌面打开最开始下载的压缩包 找到.sql后缀的文件 解压到桌面

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/658c32bf0b08a9171c8374eb96296f6a.png" alt="658c32bf0b08a9171c8374eb96296f6a" style="zoom:80%;">

然后回到主机面板

<img src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/cc4ca69f527817812e97b4689612c84c.png" title="" alt="cc4ca69f527817812e97b4689612c84c" style="zoom:50%;">

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/bbbc8fd2f531f8e20b27662e4d2a1be0.png" alt="QQ_1753713710436" style="zoom:67%;">

输入账号密码 即上张图片蓝框

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/db0184d6a6b20909ea577df8243861ea.png" alt="db0184d6a6b20909ea577df8243861ea" style="zoom:67%;">

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/e28941dd-27fc-41d1-89db-e9a5d5e50fa4.png" alt="e28941dd-27fc-41d1-89db-e9a5d5e50fa4" style="zoom:67%;">

到这里网站可以正常使用了 但是无法使用管理员后台 需要在数据库中修改管理员密码

首先将你要改的密码使用md5加密 https://www.jsongj.com/ede/md5

<img src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/9d37e157d0107ae0d9eaf624c4ad057b.png" title="" alt="9d37e157d0107ae0d9eaf624c4ad057b" style="zoom:50%;">![e147d22b0610997e2880b44e085824da](C:\Users\admin\Documents\Tencent%20Files\3537069446\nt_qq\nt_data\Pic\2025-07\Ori\e147d22b0610997e2880b44e085824da.png)

<img title="" src="https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/efa7bc12ff7bc80c9fd856610c75a761.png" alt="efa7bc12ff7bc80c9fd856610c75a761" style="zoom:67%;">

现在就全部完成了 管理员后台地址 你的域名/admin 账号admin 密码你自己设置的![98c3902125ab6481631ea753d1aaef3c](https://raw.githubusercontent.com/binghe007/123/refs/heads/main/png/98c3902125ab6481631ea753d1aaef3c.png)


