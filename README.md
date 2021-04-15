# AWStats-Themes-WebStack

一个静态网址导航网站，基于 [AWStats](https://github.com/lete114/AWStats) 静态生成器生成的静态导航网站主题

使用：[WebStack](https://github.com/WebStackPage) 模板

# 使用

> 前提是你得先克隆 [AWStats](https://github.com/lete114/AWStats) 项目，cd进入AWStats，执行下方命令克隆本项目到AWStats的themes目录下

```bash
git clone https://github.com/lete114/WebStack themes/WebStack
```

# 配置(新增网站)

打开`./themes/WebStack/config.yml`找到`menu`配置项

正常添加网站
```yml
## 菜单
menu:
  - name: 个人站点 # 分类昵称
    icon: far fa-star # 图标
    site: # 网站
      - name: Lete乐特's Blog # 网站昵称
        url: https://music.lete114.top/ # 网站地址
        img: https://www.lete114.top/img/avatar.png # 网站图标
        description: 一个喜欢记录的地方 # 网站描述
      - name: 个人主页 
        url: https://lete114.top/ 
        img: https://www.lete114.top/img/avatar.png 
        description: Lete乐特个人主页 
  - name: 开源项目
    icon: far fa-star
    site: 
      - name: Hexo-theme-MengD
        url: https://mengd.js.org/
        img: https://cdn.jsdelivr.net/gh/lete114/CDN/MengD/WindMill128.gif
        description: 一个美丽且简洁的主题 A simple, elegant, and beautiful Hexo theme
      - name: Hexo-SEO-AutoPush
        url: https://github.com/lete114/hexo-seo-autopush
        img: https://github.com/favicon.ico
        description: 每天自动提交url到百度和谷歌必应 Daily automatic submission of urls to baidu and Google bing
```

添加二级分类网站
```yml
## 菜单
menu:
  - name: 关于乐特
    icon: far fa-star
    submenu: # 子菜单
      - name: 个人站点 # 昵称
        icon: far fa-star # 图标
        site: # 网站
          - name: Lete乐特's Blog
            url: https://music.lete114.top/
            img: https://www.lete114.top/img/avatar.png
            description: 一个喜欢记录的地方
          - name: 个人主页 # 网站昵称
            url: https://lete114.top/ # 网站地址
            img: https://www.lete114.top/img/avatar.png # 网站图标
            description: Lete乐特个人主页 # 网站描述
      - name: 开源项目
        icon: far fa-star
        site: 
          - name: Hexo-theme-MengD
            url: https://mengd.js.org/
            img: https://cdn.jsdelivr.net/gh/lete114/CDN/MengD/WindMill128.gif
            description: 一个美丽且简洁的主题 A simple, elegant, and beautiful Hexo theme
          - name: Hexo-SEO-AutoPush
            url: https://github.com/lete114/hexo-seo-autopush
            img: https://github.com/favicon.ico
            description: 每天自动提交url到百度和谷歌必应 Daily automatic submission of urls to baidu and Google bing
```

# 全部配置

```yml
#--------------------------------------------------------
# AWStats-Themes-WebStack
# 项目地址：https://github.com/lete114/WebStack
# 演示地址：https://webstack.lete114.top/
# 一个静态网址导航网站
#--------------------------------------------------------

## 基础配置
title: WebStack.cc - 设计师网址导航 # 网站昵称
favicon: ./images/favicon.png # 网站图标
author: Lete乐特 # 昵称
url: http://www.webstack.cc/ #网址
color: '#e58a8a' ## 可自定义颜色(目前只跳转滚动条和回到顶部按钮) 例如：#00c4b6
image: ./images/webstack_banner_cn.png # 图片
# 关键字
keywords: UI设计,UI设计素材,设计导航,网址导航,设计资源,创意导航,创意网站导航,设计师网址大全,设计素材大全,设计师导航,UI设计资源,优秀UI设计欣赏,设计师导航,设计师网址大全,设计师网址导航,产品经理网址导航,UX师网址导航,www.webstack.cc
# 描述
description: WebStack - 收集国内外优秀设计网站、UI设计资源网站、灵感创意网站、Resources网站，定时更新分享优质产品设计书签。www.webstack.cc


# 网站logo
logo:
  expanded: ./images/logo@2x.png # 大logo
  collapsed: ./images/logo-collapsed@2x.png # 小logo

# 导航菜单
hover: desc ## 鼠标悬浮显示 网址/描述 网址：site 描述：desc
menu:
  - name: 个人站点 # 昵称
    icon: far fa-star # 图标
    site: # 网站
      - name: Lete乐特's Blog
        url: https://music.lete114.top/
        img: https://www.lete114.top/img/avatar.png
        description: 一个喜欢记录的地方
      - name: 个人主页 # 网站昵称
        url: https://lete114.top/ # 网站地址
        img: https://www.lete114.top/img/avatar.png # 网站图标
        description: Lete乐特个人主页 # 网站描述
      - name: 玩音乐
        url: https://music.lete114.top/
        img: https://www.lete114.top/img/avatar.png
        description: Lete乐特音乐
      - name: Butterfly博客
        url: https://butterfly.lete114.top/
        img: https://www.lete114.top/img/avatar.png
        description: Lete乐特Butterfly博客
      - name: Yilia博客
        url: https://yilia.lete114.top/
        img: https://www.lete114.top/img/avatar.png
        description: Lete乐特Yilia博客
  - name: 开源项目
    icon: far fa-star
    site: 
      - name: Hexo-theme-MengD
        url: https://mengd.js.org/
        img: https://cdn.jsdelivr.net/gh/lete114/CDN/MengD/WindMill128.gif
        description: 一个美丽且简洁的主题 A simple, elegant, and beautiful Hexo theme
      - name: Hexo-SEO-AutoPush
        url: https://github.com/lete114/hexo-seo-autopush
        img: https://github.com/favicon.ico
        description: 每天自动提交url到百度和谷歌必应 Daily automatic submission of urls to baidu and Google bing
      - name: SplitScreen
        url: https://github.com/lete114/SplitScreen
        img: https://github.com/favicon.ico
        description: 谷歌浏览器网站分屏插件 Website split screen is Chrome Plugins
      - name: MyBlog-Butterfly
        url: https://github.com/lete114/MyBlog-Butterfly
        img: https://github.com/favicon.ico
        description: 一个由SpringBoot写的个人博客，博客主题使用Hexo-Butterfly A personal blog written by SpringBoot uses Butterfly as the theme of the blog 
      - name: Hexo-minify
        url: https://github.com/lete114/hexo-minify
        img: https://github.com/favicon.ico
        description: Hexo resources compress HTML,CSS,JS （Hexo博客压缩，支持HTML、JS、CSS）
      - name: Hexo-theme-Yilia-Pro
        url: https://github.com/lete114/hexo-theme-yilia-pro
        img: https://github.com/favicon.ico
        description: 一个简洁优雅的hexo主题 A simple and elegant theme for hexo.
      - name: GetThemAll
        url: https://github.com/lete114/GetThemAll
        img: https://github.com/favicon.ico
        description: GetThemAll 汉化版，图片、视频、文件、链接谷歌浏览器插件批量下载器
  - name: 代码托管
    icon: far fa-star
    site:
      - name: Github
        url: https://github.com/
        img: https://github.com/favicon.ico
        description: GitHub是人们构建软件的地方。超过5000万人使用GitHub来发现、创建和贡献超过1亿个项目。
      - name: Gitee(码云)
        url: https://gitee.com/
        img: https://gitee.com/favicon.ico
        description: 码云(gitee.com)是 OSCHINA.NET 推出的代码托管平台，支持 Git 和 SVN，提供免费的私有仓库托管。目前已有超过 500 万的开发者选择码云
      - name: Coding
        url: https://coding.net/
        img: https://dn-coding-net-production-static.codehub.cn/platform/favicon.ico
        description: Coding.net 是一个面向开发者的云端开发平台，提供 Git/SVN 代码托管、任务管理、在线 WebIDE、Cloud Studio、开发协作、文件管理、Wiki 管理、提供个人服务及企业版本的服务
      - name: Vercel(ZEIT)
        url: https://vercel.com/
        img: https://assets.vercel.com/image/upload/q_auto/front/favicon/vercel/favicon.ico
        description: Coding.net 是一个面向开发者的云端开发平台，提供 Git/SVN 代码托管、任务管理、在线 WebIDE、Cloud Studio、开发协作、文件管理、Wiki 管理、提供个人服务及企业版本的服务
  - name: 编程开发
    icon: far fa-star
    site: 
      - name: How2J
        url: https://how2j.cn
        img: https://how2j.cn/favicon.ico
        description: How2J 的 Java 教程，内容涵盖 J2SE、WEB 前端、J2EE、框架技术等全面的 Java 内容。 基于实例代码和视频讲解的学习方式为 Java 职业生涯打下坚实的基础
      - name: Spring
        url: https://spring.io/
        img: https://spring.io/images/favicon.ico
        description: Spring框架是由于软件开发的复杂性而创建的。
      - name: Java
        url: http://www.java.com/
        img: https://www.java.com/favicon.ico
        description: Java是一门面向对象编程语言，不仅吸收了C++语言的各种优点，还摒弃了C++里难以理解的多继承、指针等概念，因此Java语言具有功能强大和简单易用两个特征。Java语言作为静态面向对象编程语言的代表，极好地实现了面向对象理论，允许程序员以优雅的思维方式进行复杂的编程
  - name: 阅读学习
    icon: far fa-star
    site: 
      - name: 知乎
        url: https://zhihu.com/
        img: https://zhihu.com/favicon.ico
        description: 可信赖的问答社区，以让每个人高效获得可信赖的解答为使命。
      - name: Stack Overflow
        url: https://stackoverflow.com/
        img: https://stackoverflow.com/favicon.ico
        description: Stack Overflow 是最大、最值得开发者学习的在线社区。他们的编程知识，并建立他们的职业生涯。
      - name: CSDN
        url: https://blog.csdn.net/
        img: https://blog.csdn.net/favicon.ico
        description: CSDN博客为中国软件开发者、IT从业人员、IT初学者打造交流的专业IT技术发表平台。
      - name: 掘金
        url: https://juejin.im
        img: https://juejin.im/favicon.ico
        description: 掘金是一个帮助开发者成长的社区。
      - name: Topbook
        url: https://topbook.cc/overview
        img: https://cdn.labs.topbook.cc/icon.png
        description: Topbook是一本持续更新的视频书，致力于让现代人摆脱资讯的控制。
      - name: V2MCdev
        url: https://v2mcdev.com
        img: https://v2mcdev.com/uploads/default/optimized/1X/_129430568242d1b7f853bb13ebea28b3f6af4e7_2_32x32.png
        description: 一个和 Minecraft Mod 相关的杂货论坛。
      - name: 全历史
        url: https://www.allhistory.com
        img: https://www.allhistory.com/favicon.ico
        description: 全世界，每个时期都有记载。
      - name: 今日热榜
        url: https://tophub.today
        img: https://tophub.today/favicon.ico
        description: 今日热榜提供各站热榜聚合：微信、今日头条、百度、知乎、V2EX、
      - name: 推酷
        url: https://www.tuicool.com
        img: https://static0.tuicool.com/favicon.ico
        description: 推酷网是面向IT人的个性化阅读网站，其背后的推荐引擎通过智能化的分析，向用户推荐感兴趣的科技资讯
      - name: 力扣
        url: https://leetcode-cn.com
        img: https://leetcode-cn.com/favicon.ico
        description: 备战技术面试？力扣提供海量技术面试资源，帮助你高效提升编程技能
  - name: 实用工具
    icon: far fa-star
    site: 
      - name: 小森平音效
        url: https://taira-komori.jpn.org/freesoundcn.html
        img: https://taira-komori.jpn.org/favicon.ico
        description: 免费音效可用于你想用的项目，如电影、短片、游戏、发表、动画、舞台表演、广播剧、等等...。
      - name: 网易见外工作台
        url: https://jianwai.youdao.com/
        img: https://jianwai.youdao.com/favicon.ico
        description: 支持视频、字幕、音频、文档、会议
      - name: 时光邮局
        url: https://www.hi2future.com/
        img: https://www.hi2future.com/favicon.ico
        description: 给未来的自己写一封信,问问当初的梦想是不是还在坚持;给未来的爱人写一封信,让他/她看到你十年不变的爱恋
      - name: 在线工具
        url: https://tool.lu
        img: https://tool.lu/favicon.ico
        description: 在线工具,开发人员工具,代码格式化、压缩、加密、解密
      - name: RGB颜色值HEX值
        url: http://www.ecjson.com
        img: http://www.ecjson.com/favicon.ico
        description: HEX16色转换为RGB互转工具:提供在线RGB三原色,HEX16色转换,在线RGB三原色对照表
      - name: 键盘按键值
        url: https://www.bejson.com/othertools/keycodes/
        img: http://www.bejson.com/favicon.ico
        description: 在线获取键盘按键值
      - name: Color Hunt
        url: https://colorhunt.co
        img: https://colorhunt.co/img/favicon.gif
        description: Color Hunt 是一个免费和开放的平台，为色彩灵感与数以千计的时尚的手选调色板
      - name: 字由
        url: https://www.hellofont.cn
        img: https://www.hellofont.cn/favicon.ico
        description:  字由是为设计师量身定做的一款字体下载管理工具
      - name: ASCII 在线转换器
        url: https://www.sojson.com/ascii.html
        img: http://cdn.yinshua86.com/sojson/favicon.ico
        description:  本工具是根据 ASCII 表做对应转码操作，转换完成后即可看到对应的内容，ASCII 码一般用于配置文件防止乱码使用。
      - name: banner 在线生成工具
        url: https://www.bootschool.net/ascii
        img: https://www.bootschool.net/site/images/favico.png
        description:  springboot banner 工具实现在线生成 banner，是很棒的 springboot banner 自定义和命令行 ascii 文字工具。有了它你的项目会变得有意思
  - name: 图片美图
    icon: far fa-star
    site: 
      - name: Textures for 3D
        url: https://www.textures.com
        img: https://www.textures.com/favicon.ico
        description: 纹理为 3D，图形设计和 Photoshop!
      - name: Streetwill
        url: http://www.streetwill.co
        img: http://www.streetwill.co/favicon.png
        description: 每天都有好看的壁纸图片！！
      - name: BoBoPic
        url: https://bobopic.com/
        img: https://tu.bobopic.com/static/img/favicon.ico
        description: 每天都有好看的壁纸图片！！
      - name: 以图搜动漫
        url: https://trace.moe/
        img: https://trace.moe/favicon.png
        description: 只有图片，不知道动漫名？用它秒找动漫
      - name: 动漫画风的云
        url: https://www.ianfisherart.com/
        img: https://www.ianfisherart.com/favicon.ico
        description: 动漫画风的云 Ian Fisher
  - name: 免费API
    icon: far fa-star
    site: 
      - name: 搏天 api - 免费 api 接口平台
        url: https://api.btstu.cn
        img: https://api.btstu.cn/favicon.ico
        description: 搏天 api, 免费 api,api,api 接口，免费 api 接口，缥缈，随机二次元壁纸 api, 随机美女壁纸 api, 短网址生成 api
      - name: 保罗｜API
        url: https://api.paugram.com/
        img: https://api.paugram.com/static/img/icon.png
        description: 奇趣保罗,鲍小螺,保罗,Dreamer-Paul,dreamer-paul,Paul,paul
      - name: 墨天逸 — 随机图片API
        url: https://api.mtyqx.cn/
        img: https://api.mtyqx.cn/favicon.ico
        description: 随机图片API
      - name: 网易云音乐 NodeJS 版 API
        url: https://binaryify.github.io/NeteaseCloudMusicApi
        img: https://binaryify.github.io/NeteaseCloudMusicApi/favicon.ico
        description: 网易云音乐 NodeJS 版 API
      - name: 韩小韩api
        url: https://api.vvhan.com/
        img: https://api.vvhan.com/favicon.ico
        description: 韩小韩api接口 - 一个免费的api接口网站
      - name: Ten▪Api
        url: https://tenapi.cn/
        img: https://tenapi.cn/favicon.ico
        description: 韩小韩api接口 - 一个免费的api接口网站


# 搜索功能
search: 
  enable: true # 是否开启
  default_search_source: https://www.baidu.com/s?wd= ## 默认搜索平台
  default_search_icon: ./images/search/baidu.ico ## 默认搜索图标
  search_source: # 搜索源
    - name: 百度 # 昵称
      img: ./images/search/baidu.ico # 源图标
      url: https://www.baidu.com/s?wd= # 搜索平台的请求地址
    - name: 谷歌
      img: ./images/search/google.ico
      url: https://www.google.com/search?q=
    - name: 必应
      img: ./images/search/bing.ico
      url: https://cn.bing.com/search?q=
    - name: 好搜
      img: ./images/search/360.ico
      url: https://www.so.com/s?q=
    - name: 搜狗
      img: ./images/search/sogou.ico
      url: https://www.sogou.com/web?query=
    - name: 淘宝
      img: ./images/search/taobao.ico
      url: https://s.taobao.com/search?q=
    - name: 京东
      img: ./images/search/JD.ico
      url: http://search.jd.com/Search?keyword=
    - name: 天猫
      img: ./images/search/tianmao.ico
      url: https://list.tmall.com/search_product.htm?q=
    - name: "1688" ## 如果是数字推荐使用双引号 "" 包起来(不用双引号也可以)
      img: ./images/search/1688.ico
      url: https://s.1688.com/selloffer/offer_search.htm?keywords=
    - name: 知乎
      img: ./images/search/zhihu.ico
      url: https://www.zhihu.com/search?type=content&q=
    - name: 微博
      img: ./images/search/weibo.ico
      url: https://s.weibo.com/weibo/
    - name: B站
      img: ./images/search/bilibili.ico
      url: http://search.bilibili.com/all?keyword=
    - name: 豆瓣
      img: ./images/search/douban.ico
      url: https://www.douban.com/search?source=suggest&q=
    - name: 优酷
      img: ./images/search/youku.ico
      url: https://so.youku.com/search_video/q_
    - name: GitHub
      img: ./images/search/github.ico
      url: https://github.com/search?utf8=✓&q=

since: 2020 # 网站开启时间

## 404页面
error_404:
  title: webstack - 404 # 标题
  subtitle: Oops! It looks like you're lost... # 副标题
  description: The Page you're looking for doesn't exist or another error occurred. # 描述
  return: webstack.cc # 返回的域名(网址)

# 访问量统计
busuanzi:
  enable: true
  pv: 本站总访问量$pv
  uv: 本站总访客数$uv

# 分析(统计)
analytics:
  baidu: # 百度分析
  google: # 谷歌分析

CDN:
  fontawesome: ./css/fonts/fontawesome/css/font-awesome.min.css
  bootstrap_css: ./css/bootstrap.css
  bootstrap_js: https://cdn.jsdelivr.net/npm/bootstrap@3.3.1/dist/js/bootstrap.min.js
  xenon_core: ./css/xenon-core.css
  xenon_components: ./css/xenon-components.css
  nav: ./css/nav.css
  jQuery: https://cdn.jsdelivr.net/npm/jquery@latest/dist/jquery.min.js

  # search
  search_js: ./js/search.js
  search_css: ./css/search.css

  # 不蒜子
  busuanzi: https://busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js

  TweenMax: ./js/TweenMax.min.js
  resizeable: ./js/resizeable.js
  joinable: ./js/joinable.js
  xenon_api: ./js/xenon-api.js
  xenon_toggles: ./js/xenon-toggles.js
  xenon_custom: ./js/xenon-custom.js
  lozad: https://cdn.jsdelivr.net/npm/lozad/dist/lozad.min.js
```
