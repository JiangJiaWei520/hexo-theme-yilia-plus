hexo-theme-yilia-plus
================

 &#160;此项目是根据[hexo-theme-yilia](https://github.com/litten/hexo-theme-yilia)主题做了一些优化和改动，使用`yilia`主题可以快速迁移到`yilia-plus`

#### [立即体验](#三开始使用)

## 关于[hexo-theme-yilia-plus](https://github.com/JoeyBling/hexo-theme-yilia-plus)主题功能
1. 手机端头像添加主页跳转链接
2. 集成不蒜子访问量统计功能
3. 网易云音乐插件
4. 页面点击小红心效果
5. 增加了多个SubNav导航图标展示
6. 添加GitHub Ribbons(Fork me)
7. 页脚 Litten自定义(弃用)
8. 添加版权声明
9. 添加百度站长平台主动推送
10. 集成 gitment 评论 ➡️ [https://github.com/JoeyBling/yilia-plus-demo](https://github.com/JoeyBling/yilia-plus-demo)
11. [集成码云评论](https://gitee.com/zhousiwei/giteement) ➡️ [https://gitee.com/zhousiwei/yilia-plus-demo](https://gitee.com/zhousiwei/yilia-plus-demo)
12. 添加网站成立年份
13. 页面加载进度条
14. 添加苹果图标
15. 标签页标题切换功能
16. 添加字数统计功能
17. 添加文字输入特效
18. 友情链接优化展示
19. 左侧边栏动态图效果、左侧导航栏支持滚动
20. 添加悬停预览图片效果
21. 其他样式轻微调优、社交图标优化
22. 优化配置是否在新窗口打开链接
23. [fix bugs](https://github.com/JoeyBling/hexo-theme-yilia-plus/wiki/fix-bugs-record%EF%BC%88%E4%BF%AE%E5%A4%8Dbug%E8%AE%B0%E5%BD%95%EF%BC%89)
24. [添加看板娘动态模型插件](https://github.com/JoeyBling/live2d-widget.js)
25. 添加飘雪特效
26. 自定义文章版权声明文本

> 如果有小伙伴有新功能的意见或者改进欢迎给我提意见和建议~

## 一、外观

#### **常规**

![常规](https://github.com/JiangJiaWei520/hexo-theme-yilia-plus/raw/master/examples/images/web.png)

## 二、开发者

#### 评论支持
- [Gitment](https://github.com/imsun/gitment)
- [基于码云的评论系统](https://gitee.com/zhousiwei/giteement)
- DISQUS
- 搜狐畅言

## 三、开始使用

#### 1、安装

```bash
cd ./themes/
git clone --depth=1 https://github.com/JiangJiaWei520/hexo-theme-yilia-plus.git ./yilia-plus
```

#### 2、配置

修改hexo根目录下的 `_config.yml`  ➡️  `theme: yilia-plus`

#### 3、更新

```bash
cd themes/yilia-plus
git pull
```

## 四、配置

### 1)基本功能&#160;&#160;&#160;

&#160;主题配置文件在主目录下的`_config.yml`，请根据自己需要修改使用。

> 完整配置Demo例子，可以参考[yilia-plus博客备份](http://github.com/JoeyBling/yilia-plus-demo)

```yaml
# Header-菜单,/tags/-->_posts
menu:
  主页: /
  技术笔记: https://zhousiwei.gitee.io/ibooks/
  随笔: /tags/随笔/
  #photos: /photos

# subNav-子导航
subNav:
  github: "#"
  gitee: "#" # 码云
  jianshu: "#" #简书
  cnblog: "#"
  #blog: "#"
  #csdn: "#"
  #rss: "#"
  #zhihu: "#"
  #qq: "img/2434387555.jpg"
  #weixin: "img/weixin_.png"
  #weibo: "#"
  #douban: "#"
  #segmentfault: "#"
  #bilibili: "#"
  #acfun: "#"
  #mail: "mailto:zhousiwei0911@qq.com"
  #facebook: "#"
  #google: "#"
  #twitter: "#"
  #linkedin: "#"

# 悬停预览图片效果
hover_effect:
  ## `global` 0: Set separately, 1: Enable global 2: Close global
  ## `global` 0: 分开设置, 1: 全局启用, 2: 全局关闭
  global: 2
  # SubNav-导航
  subNav: true

# RSS订阅(关于如何配置启用:https://www.jianshu.com/p/2aaac7a19736)
rss: /atom.xml

# 是否需要修改 root 路径
# 如果您的网站存放在子目录中，例如 http://yoursite.com/blog，
# 请将您的 url 设为 http://yoursite.com/blog 并把 / 设为 /blog/。
root: /

# Content

# 文章太长，截断按钮文字(在需要截断的行增加此标记：<!--more-->)
excerpt_link: more
# 文章卡片右下角常驻链接，不需要请设置为false
show_all_link: '展开全文'
# 数学公式
mathjax: false

# Open link in a new tab | 是否在新窗口打开链接
open_in_new:
  article: true  # 文章链接
  menu: true   # 导航菜单
  subNav: true  # 子菜单

# 打赏
# 打赏type设定：0-关闭打赏； 1-文章对应的md文件里有reward:true属性，才有打赏； 2-所有文章均有打赏
reward_type: 2
# 打赏wording
reward_wording: '谢谢你请我吃糖果'
# 支付宝二维码图片地址，跟你设置头像的方式一样。比如：/assets/img/alipay.jpg
alipay: /img/alipay.jpg
# 微信二维码图片地址
weixin: /img/weixin.png

# 目录
# 目录设定：0-不显示目录； 1-文章对应的md文件里有toc:true属性，才有目录； 2-所有文章均显示目录
toc: 1
# 根据自己的习惯来设置，如果你的目录标题习惯有标号，置为true即可隐藏hexo重复的序号；否则置为false
toc_hide_index: true
# 目录为空时的提示
toc_empty_wording: '目录，不存在的…'

# 是否有快速回到顶部的按钮
top: true

# Miscellaneous
# 百度统计
baidu_analytics: ''
google_analytics: ''

# 网站图标
favicon: /favicon.ico

# 你的头像url
avatar: /img/head.jpg

# 是否开启分享
share_jia: true

# 评论：1、畅言；2、Disqus；3、Gitment；4、Giteement
# 不需要使用某项，直接设置值为false，或注释掉
# 具体请参考wiki：https://github.com/JoeyBling/hexo-theme-yilia-plus/wiki

# 1、畅言
changyan_appid: false
changyan_conf: false

# 2、Disqus 在hexo根目录的config里也有disqus_shortname字段，优先使用yilia-plus的
disqus: false

# 3、Gitment----基于GitHub的评论系统(关闭请设置gitment_owner为false)
# 关于如何集成:https://www.jianshu.com/p/ac7658cc912f
gitment_owner: false      #你的 GitHub ID
# 是否使用官方js(false可以提升访问速度，本地修改过一部分的js，官方js可能会出现服务器不稳定，不太建议使用)
gitment_remote: false
gitment_repo: ''          #存储评论的 repo name(需要在Github创建)
gitment_oauth:
  client_id: ''           #client ID
  client_secret: ''       #client secret

# 4、Giteement----【国内用户建议使用这个，相对比较快】
# 关于如何集成:https://www.jianshu.com/p/f5c4633524c7
# 基于码云的评论系统(https://gitee.com/zhousiwei/giteement)
giteement:
  enable: false  # 是否启用码云评论系统
  # 是否使用官方js(false可以提升访问速度)
  remote: false
  redirect_uri: ''   # 应用回调地址(请和配置的第三方应用保持一致)
  # 不能更改(网上开源项目`https://github.com/Rob--W/cors-anywhere`作者提供的专门用来跨域服务器的配置)
  oauth_uri: https://cors-anywhere.herokuapp.com/https://gitee.com/oauth/token
  giteeID: ''  # 你的码云账号英文名
  # 存储评论的 repo name(需要在码云仓库创建公开仓库)
  repo: ''
  gitment_oauth:
    client_id: ''           #client ID
    client_secret: ''       #client secret

# 访问量统计功能(不蒜子)
busuanzi:
  enable: true
  site_visit: true  # 站点访问量显示
  article_visit: true  # 文章访问量显示

# 网易云音乐插件
music:
  enable: false
  # 播放器尺寸类型(1：长尺寸、2：短尺寸)
  type: 2
  #id: 1332647902  # 网易云分享的音乐ID(更换音乐请更改此配置项)
  autoPlay: true  # 是否开启自动播放
  # 提示文本(关闭请设置为false)
  text: '这似乎是首纯音乐，请尽情的欣赏它吧！'

# 页面点击小红心
clickLove:
  # (关闭请设置为false)
  enable: true

# GitHub Ribbons(https://github.blog/2008-12-19-github-ribbons/)
github:
  # (关闭请设置为false)
  url: https://github.com/JoeyBling/hexo-theme-yilia-plus

# 页脚 Litten(此配置项已弃用)
# 帮助我们让更多人可以更方便使用Hexo，请尽量不要修改此主题配置
pageFooter:
  litten: GitHub:<a href="https://github.com/JoeyBling/hexo-theme-yilia-plus" target="_blank">hexo-theme-yilia-plus</a>

# 开启百度站长平台自动推送(https://ziyuan.baidu.com/linksubmit/index)
baidu_push: false

# 版权声明
# 版权声明type设定：0-关闭版权声明； 1-文章对应的md文件里有copyright: true属性，才有版权声明； 2-所有文章均有版权声明
copyright_type: 2

# 网站成立年份(默认为 2018，若填入年份小于当前年份，则显示为 2018-2019 类似的格式)
since: 2018

# Progress Bar | 页面加载进度条
# Demo: http://github.hubspot.com/pace/docs/welcome/
# type: barber-shop|big-counter|bounce|center-atom|center-circle|
#       center-radar|center-simple|corner-indicator|flash|flat-top|
#       loading-bar|mac-osx|minimal
# color: black|blue|green|orange|pink|purple|red|silver|white|yellow|
progressBar:
  enable: false
  type: 'minimal'  # Keep Quotes | 保留引号避免出错(某些type会导致样式重叠排版错误)
  color: blue

# Apple Touch icon 苹果图标(关闭请设置为false)
apple_touch_icon: '/apple-touch-icon-180x180.png'

# Tab Title Change | 标签页标题切换
tab_title_change:
  enable: true
  left_tab_title: '(つェ⊂) 我藏好了哦~ '
  return_tab_title: '(*´∇｀*) 被你发现啦~ '

# https://github.com/willin/hexo-wordcount
# 是否开启字数统计(关闭请设置enable为false)
# 也可以单独在md文件里Front-matter设置`no_word_count: true`属性，来自定义关闭字数统计
word_count:
  enable: true
  # 只在文章详情显示(不在首页显示)
  only_article_visit: true

# 文字输入特效
# https://github.com/disjukr/activate-power-mode
activate_power_mode:
  enable: true
  # 使输入模式丰富多彩
  colorful: true
  # 是否开启摇动
  shake: false

# 飘雪特效
# https://github.com/MlgmXyysd/snow.js
snow: false

# 看板娘动态模型插件
## https://github.com/JoeyBling/live2d-widget.js
live2d:
  # (关闭请设置为false)
  enable: false
  # 模型名称(取值请参考：https://github.com/JoeyBling/hexo-theme-yilia-plus/wiki/live2d%E6%A8%A1%E5%9E%8B%E5%8C%85%E5%B1%95%E7%A4%BA)
  model: hibiki
  display:
    position: right # 显示位置：left/right(default: 'right')
    width: 145  # 模型的长度(default: 150)
    height: 315 # 模型的高度(default: 300)
    hOffset: 50 # 水平偏移(default: 0)
    #vOffset: -20 # 垂直偏移(default: -20)
  mobile:
    show: false # 是否在移动设备上显示(default: true)
    scale: 0.6 # 移动设备上的缩放(default: 0.5)
  react:
    opacity: 0.8 # 模型透明度(default: 0.7)

# 样式定制 - 一般不需要修改，除非有很强的定制欲望…
style:
  # 头像上面的背景颜色
  # header: '#D3D1DC'
  header: '#4d4d4d'
  gif:
    # 是否启用左侧边栏动态图效果
    enable: false
    # 自定义背景图路径(默认可以不设置，提供默认背景图)
    # path: /img/biubiubiu.gif
  # 右滑板块背景
  slider: 'linear-gradient(200deg,#a0cfe4,#e8c37e)'

# slider的设置
slider:
  # 是否默认展开tags板块
  showTags: false

# 智能菜单
# 如不需要，将该对应项置为false
# 比如
#smart_menu:
#  friends: false
smart_menu:
  innerArchive: '所有文章'
  friends: '友链'
  aboutme: '关于我'

# 友情链接
friends:
  技术笔记:  #网站名称
    #网站地址
    url: https://zhousiwei.gitee.io/ibooks/
    #网站图片(可忽略不写)
    img: https://zhousiwei.gitee.io/ibooks/favicon.ico
    #网站简介(可忽略不写)
    description: 记录工作和学习过程中的笔记：Java、前端开发、Hexo博客、聚合支付、Linux笔记、ElasticSearch、ELK日志分析
  GitHub:
    url: https://github.com/JoeyBling
  码云:
    url: https://gitee.com/zhousiwei
  简书:
    url: https://www.jianshu.com/u/02cbf31a043a
  CSDN:
    url: https://blog.csdn.net
```

### 2)添加音乐播放器

[梨花带雨播放器]: https://music.m0x.cn

### 3)点击特效

今天浏览到一个网站，发现在网页上点击的时候，会依次出现社会主义核心价值观。觉的很有意思，就把代码偷过来了。就是一个JavaScript脚本。

然后把它添加到博客的模板文件里。

在layouts`文件夹里。找一下看看哪个html文件里`<head>`和`<body>`，大概率就是博客的主模板文件了。然后拉到最后，在`</body>`上面插入下面任意一个代码。

```
themes\yilia-plus\layout\_partial\footer.ejs
```

#### A.鼠标点击心形特效

```
<script>
		(function(window,document,undefined){
			var hearts = [];
			window.requestAnimationFrame = (function(){
				return window.requestAnimationFrame ||
				window.webkitRequestAnimationFrame ||
				window.mozRequestAnimationFrame ||
				window.oRequestAnimationFrame ||
				window.msRequestAnimationFrame ||
				function (callback){
					setTimeout(callback,1000/60);
				}
			})();
			init();
			function init(){
				css(".heart{width: 10px;height: 10px;position: fixed;background: #f00;transform: rotate(45deg);-webkit-transform: rotate(45deg);-moz-transform: rotate(45deg);}.heart:after,.heart:before{content: '';width: inherit;height: inherit;background: inherit;border-radius: 50%;-webkit-border-radius: 50%;-moz-border-radius: 50%;position: absolute;}.heart:after{top: -5px;}.heart:before{left: -5px;}");
				attachEvent();
				gameloop();
			}
			function gameloop(){
				for(var i=0;i<hearts.length;i++){
					if(hearts[i].alpha <=0){
						document.body.removeChild(hearts[i].el);
						hearts.splice(i,1);
						continue;
					}
					hearts[i].y--;
					hearts[i].scale += 0.004;
					hearts[i].alpha -= 0.013;
					hearts[i].el.style.cssText = "left:"+hearts[i].x+"px;top:"+hearts[i].y+"px;opacity:"+hearts[i].alpha+";transform:scale("+hearts[i].scale+","+hearts[i].scale+") rotate(45deg);background:"+hearts[i].color;
				}
				requestAnimationFrame(gameloop);
			}
			function attachEvent(){
				var old = typeof window.οnclick==="function" && window.onclick;
				window.onclick = function(event){
					old && old();
					createHeart(event);
				}
			}
			function createHeart(event){
				var d = document.createElement("div");
				d.className = "heart";
				hearts.push({
					el : d,
					x : event.clientX - 5,
					y : event.clientY - 5,
					scale : 1,
					alpha : 1,
					color : randomColor()
				});
				document.body.appendChild(d);
			}
			function css(css){
				var style = document.createElement("style");
				style.type="text/css";
				try{
					style.appendChild(document.createTextNode(css));
				}catch(ex){
					style.styleSheet.cssText = css;
				}
				document.getElementsByTagName('head')[0].appendChild(style);
			}
			function randomColor(){
				return "rgb("+(~~(Math.random()*255))+","+(~~(Math.random()*255))+","+(~~(Math.random()*255))+")";
			}
		})(window,document);
</script>
```

#### B. 鼠标点击社会主义核心价值观特效

```
<script src="https://cdn.bootcss.com/jquery/3.3.1/jquery.min.js"></script>
<script type="text/javascript">
        /* 鼠标点击特效 - 7Core.CN */
        var a_idx = 0;jQuery(document).ready(function($) {$("body").click(function(e) {var a = new Array("富强", "民主", "文明", "和谐", "自由", "平等", "公正" ,"法治", "爱国", "敬业", "诚信", "友善");var $i = $("<span/>").text(a[a_idx]);
        a_idx = (a_idx + 1) % a.length;var x = e.pageX,y = e.pageY;$i.css({"z-index": 100000000,"top": y - 20,"left": x,"position": "absolute","font-weight": "bold","color": "#ff6651"});$("body").append($i);$i.animate({"top": y - 180,"opacity": 0},1500,function() {$i.remove();});});});
</script>
```

或者

```
<script type="text/javascript">
/* 鼠标特效 */
var a_idx = 0;
jQuery(document).ready(function($) {
    $("body").click(function(e) {
        var a = new Array("❤凯鲁嘎吉❤","❤爱你❤","❤欢迎您❤","❤光临本园❤","❤加油❤","❤努力❤","❤奋斗❤","❤拼搏❤","❤凯鲁嘎吉❤","❤爱你❤","❤forever❤","❤爱你❤");
        var $i = $("<span></span>").text(a[a_idx]);
        a_idx = (a_idx + 1) % a.length;
        var x = e.pageX,
        y = e.pageY;
        $i.css({
            "z-index": 999999999999999999999999999999999999999999999999999999999999999999999,
            "top": y - 20,
            "left": x,
            "position": "absolute",
            "font-weight": "bold",
            "color": "rgb("+~~(255*Math.random())+","+~~(255*Math.random())+","+~~(255*Math.random())+")"
        });
        $("body").append($i);
        $i.animate({
            "top": y - 180,
            "opacity": 0
        },
        1500,
        function() {
            $i.remove();
        });
    });
});
</script>
```

#### C. 鼠标环绕特效

```
<section ></section>
<script type='text/javascript'>
!function () { function o(w, v, i) { return w.getAttribute(v) || i } function j(i) { return document.getElementsByTagName(i) } function l() { var i = j("script"), w = i.length, v = i[w - 1]; return { l: w, z: o(v, "zIndex", -1), o: o(v, "opacity", 0.5), c: o(v, "color", "0,0,0"), n: o(v, "count", 99) } } function k() { r = u.width = window.innerWidth || document.documentElement.clientWidth || document.body.clientWidth, n = u.height = window.innerHeight || document.documentElement.clientHeight || document.body.clientHeight } function b() { e.clearRect(0, 0, r, n); var w = [f].concat(t); var x, v, A, B, z, y; t.forEach(function (i) { i.x += i.xa, i.y += i.ya, i.xa *= i.x > r || i.x <0 ? -1 : 1, i.ya *=i.y>n || i.y <0 ? -1 : 1, e.fillRect(i.x - 0.5, i.y - 0.5, 1, 1); for (v=0; v < w.length; v++) { x = w[v]; if (i !== x &&null !== x.x &&null !== x.y) { B = i.x - x.x, z = i.y - x.y, y = B * B + z * z; y <x.max && (x=== f && y>= x.max / 2 &&(i.x -= 0.03 * B, i.y -= 0.03 * z), A = (x.max - y) / x.max, e.beginPath(), e.lineWidth = A / 2, e.strokeStyle = "rgba(" + s.c + "," + (A + 0.2) + ")", e.moveTo(i.x, i.y), e.lineTo(x.x, x.y), e.stroke()) } } w.splice(w.indexOf(i), 1) }), m(b) } var u = document.createElement("canvas"),  s = l(), c = "c_n" + s.l, e = u.getContext("2d"), r, n, m = window.requestAnimationFrame || window.webkitRequestAnimationFrame || window.mozRequestAnimationFrame || window.oRequestAnimationFrame || window.msRequestAnimationFrame || function (i) { window.setTimeout(i, 1000 / 45) }, a = Math.random, f = { x: null, y: null, max: 20000 }; u.id = c; u.className = "hidden-xs hidden-sm my_canvas"; u.style.cssText = "position:fixed;top:0;left:0;z-index:" + s.z + ";opacity:" + s.o; j("body")[0].appendChild(u); k(), window.onresize = k; window.onmousemove = function (i) { i = i || window.event, f.x = i.clientX, f.y = i.clientY }, window.onmouseout = function () { f.x = null, f.y = null }; for (var t = [], p = 0; s.n > p; p++) { var h = a() * r, g = a() * n, q = 2 * a() - 1, d = 2 * a() - 1; t.push({ x: h, y: g, xa: q, ya: d, max: 6000 }) } setTimeout(function () { b() }, 100) }();
</script>
```

> 我也不知道第一行的<section ></section>是要干嘛，但是确实删了就不正常显示了。。。。

#### D.点击爆炸特效

```
<canvas class="fireworks" style="position:fixed;left:0;top:0;z-index:99999999;pointer-events:none;"> 
</canvas>
<script  type="text/javascript">
/*
 2017 Julian Garnier
 Released under the MIT license
*/
var $jscomp={scope:{}};$jscomp.defineProperty="function"==typeof Object.defineProperties?Object.defineProperty:function(e,r,p){if(p.get||p.set)throw new TypeError("ES3 does not support getters and setters.");e!=Array.prototype&&e!=Object.prototype&&(e[r]=p.value)};$jscomp.getGlobal=function(e){return"undefined"!=typeof window&&window===e?e:"undefined"!=typeof global&&null!=global?global:e};$jscomp.global=$jscomp.getGlobal(this);$jscomp.SYMBOL_PREFIX="jscomp_symbol_";
$jscomp.initSymbol=function(){$jscomp.initSymbol=function(){};$jscomp.global.Symbol||($jscomp.global.Symbol=$jscomp.Symbol)};$jscomp.symbolCounter_=0;$jscomp.Symbol=function(e){return $jscomp.SYMBOL_PREFIX+(e||"")+$jscomp.symbolCounter_++};
$jscomp.initSymbolIterator=function(){$jscomp.initSymbol();var e=$jscomp.global.Symbol.iterator;e||(e=$jscomp.global.Symbol.iterator=$jscomp.global.Symbol("iterator"));"function"!=typeof Array.prototype[e]&&$jscomp.defineProperty(Array.prototype,e,{configurable:!0,writable:!0,value:function(){return $jscomp.arrayIterator(this)}});$jscomp.initSymbolIterator=function(){}};$jscomp.arrayIterator=function(e){var r=0;return $jscomp.iteratorPrototype(function(){return r<e.length?{done:!1,value:e[r++]}:{done:!0}})};
$jscomp.iteratorPrototype=function(e){$jscomp.initSymbolIterator();e={next:e};e[$jscomp.global.Symbol.iterator]=function(){return this};return e};$jscomp.array=$jscomp.array||{};$jscomp.iteratorFromArray=function(e,r){$jscomp.initSymbolIterator();e instanceof String&&(e+="");var p=0,m={next:function(){if(p<e.length){var u=p++;return{value:r(u,e[u]),done:!1}}m.next=function(){return{done:!0,value:void 0}};return m.next()}};m[Symbol.iterator]=function(){return m};return m};
$jscomp.polyfill=function(e,r,p,m){if(r){p=$jscomp.global;e=e.split(".");for(m=0;m<e.length-1;m++){var u=e[m];u in p||(p[u]={});p=p[u]}e=e[e.length-1];m=p[e];r=r(m);r!=m&&null!=r&&$jscomp.defineProperty(p,e,{configurable:!0,writable:!0,value:r})}};$jscomp.polyfill("Array.prototype.keys",function(e){return e?e:function(){return $jscomp.iteratorFromArray(this,function(e){return e})}},"es6-impl","es3");var $jscomp$this=this;
(function(e,r){"function"===typeof define&&define.amd?define([],r):"object"===typeof module&&module.exports?module.exports=r():e.anime=r()})(this,function(){function e(a){if(!h.col(a))try{return document.querySelectorAll(a)}catch(c){}}function r(a,c){for(var d=a.length,b=2<=arguments.length?arguments[1]:void 0,f=[],n=0;n<d;n++)if(n in a){var k=a[n];c.call(b,k,n,a)&&f.push(k)}return f}function p(a){return a.reduce(function(a,d){return a.concat(h.arr(d)?p(d):d)},[])}function m(a){if(h.arr(a))return a;
h.str(a)&&(a=e(a)||a);return a instanceof NodeList||a instanceof HTMLCollection?[].slice.call(a):[a]}function u(a,c){return a.some(function(a){return a===c})}function C(a){var c={},d;for(d in a)c[d]=a[d];return c}function D(a,c){var d=C(a),b;for(b in a)d[b]=c.hasOwnProperty(b)?c[b]:a[b];return d}function z(a,c){var d=C(a),b;for(b in c)d[b]=h.und(a[b])?c[b]:a[b];return d}function T(a){a=a.replace(/^#?([a-f\d])([a-f\d])([a-f\d])$/i,function(a,c,d,k){return c+c+d+d+k+k});var c=/^#?([a-f\d]{2})([a-f\d]{2})([a-f\d]{2})$/i.exec(a);
a=parseInt(c[1],16);var d=parseInt(c[2],16),c=parseInt(c[3],16);return"rgba("+a+","+d+","+c+",1)"}function U(a){function c(a,c,b){0>b&&(b+=1);1<b&&--b;return b<1/6?a+6*(c-a)*b:.5>b?c:b<2/3?a+(c-a)*(2/3-b)*6:a}var d=/hsl\((\d+),\s*([\d.]+)%,\s*([\d.]+)%\)/g.exec(a)||/hsla\((\d+),\s*([\d.]+)%,\s*([\d.]+)%,\s*([\d.]+)\)/g.exec(a);a=parseInt(d[1])/360;var b=parseInt(d[2])/100,f=parseInt(d[3])/100,d=d[4]||1;if(0==b)f=b=a=f;else{var n=.5>f?f*(1+b):f+b-f*b,k=2*f-n,f=c(k,n,a+1/3),b=c(k,n,a);a=c(k,n,a-1/3)}return"rgba("+
255*f+","+255*b+","+255*a+","+d+")"}function y(a){if(a=/([\+\-]?[0-9#\.]+)(%|px|pt|em|rem|in|cm|mm|ex|ch|pc|vw|vh|vmin|vmax|deg|rad|turn)?$/.exec(a))return a[2]}function V(a){if(-1<a.indexOf("translate")||"perspective"===a)return"px";if(-1<a.indexOf("rotate")||-1<a.indexOf("skew"))return"deg"}function I(a,c){return h.fnc(a)?a(c.target,c.id,c.total):a}function E(a,c){if(c in a.style)return getComputedStyle(a).getPropertyValue(c.replace(/([a-z])([A-Z])/g,"$1-$2").toLowerCase())||"0"}function J(a,c){if(h.dom(a)&&
u(W,c))return"transform";if(h.dom(a)&&(a.getAttribute(c)||h.svg(a)&&a[c]))return"attribute";if(h.dom(a)&&"transform"!==c&&E(a,c))return"css";if(null!=a[c])return"object"}function X(a,c){var d=V(c),d=-1<c.indexOf("scale")?1:0+d;a=a.style.transform;if(!a)return d;for(var b=[],f=[],n=[],k=/(\w+)\((.+?)\)/g;b=k.exec(a);)f.push(b[1]),n.push(b[2]);a=r(n,function(a,b){return f[b]===c});return a.length?a[0]:d}function K(a,c){switch(J(a,c)){case "transform":return X(a,c);case "css":return E(a,c);case "attribute":return a.getAttribute(c)}return a[c]||
0}function L(a,c){var d=/^(\*=|\+=|-=)/.exec(a);if(!d)return a;var b=y(a)||0;c=parseFloat(c);a=parseFloat(a.replace(d[0],""));switch(d[0][0]){case "+":return c+a+b;case "-":return c-a+b;case "*":return c*a+b}}function F(a,c){return Math.sqrt(Math.pow(c.x-a.x,2)+Math.pow(c.y-a.y,2))}function M(a){a=a.points;for(var c=0,d,b=0;b<a.numberOfItems;b++){var f=a.getItem(b);0<b&&(c+=F(d,f));d=f}return c}function N(a){if(a.getTotalLength)return a.getTotalLength();switch(a.tagName.toLowerCase()){case "circle":return 2*
Math.PI*a.getAttribute("r");case "rect":return 2*a.getAttribute("width")+2*a.getAttribute("height");case "line":return F({x:a.getAttribute("x1"),y:a.getAttribute("y1")},{x:a.getAttribute("x2"),y:a.getAttribute("y2")});case "polyline":return M(a);case "polygon":var c=a.points;return M(a)+F(c.getItem(c.numberOfItems-1),c.getItem(0))}}function Y(a,c){function d(b){b=void 0===b?0:b;return a.el.getPointAtLength(1<=c+b?c+b:0)}var b=d(),f=d(-1),n=d(1);switch(a.property){case "x":return b.x;case "y":return b.y;
case "angle":return 180*Math.atan2(n.y-f.y,n.x-f.x)/Math.PI}}function O(a,c){var d=/-?\d*\.?\d+/g,b;b=h.pth(a)?a.totalLength:a;if(h.col(b))if(h.rgb(b)){var f=/rgb\((\d+,\s*[\d]+,\s*[\d]+)\)/g.exec(b);b=f?"rgba("+f[1]+",1)":b}else b=h.hex(b)?T(b):h.hsl(b)?U(b):void 0;else f=(f=y(b))?b.substr(0,b.length-f.length):b,b=c&&!/\s/g.test(b)?f+c:f;b+="";return{original:b,numbers:b.match(d)?b.match(d).map(Number):[0],strings:h.str(a)||c?b.split(d):[]}}function P(a){a=a?p(h.arr(a)?a.map(m):m(a)):[];return r(a,
function(a,d,b){return b.indexOf(a)===d})}function Z(a){var c=P(a);return c.map(function(a,b){return{target:a,id:b,total:c.length}})}function aa(a,c){var d=C(c);if(h.arr(a)){var b=a.length;2!==b||h.obj(a[0])?h.fnc(c.duration)||(d.duration=c.duration/b):a={value:a}}return m(a).map(function(a,b){b=b?0:c.delay;a=h.obj(a)&&!h.pth(a)?a:{value:a};h.und(a.delay)&&(a.delay=b);return a}).map(function(a){return z(a,d)})}function ba(a,c){var d={},b;for(b in a){var f=I(a[b],c);h.arr(f)&&(f=f.map(function(a){return I(a,
c)}),1===f.length&&(f=f[0]));d[b]=f}d.duration=parseFloat(d.duration);d.delay=parseFloat(d.delay);return d}function ca(a){return h.arr(a)?A.apply(this,a):Q[a]}function da(a,c){var d;return a.tweens.map(function(b){b=ba(b,c);var f=b.value,e=K(c.target,a.name),k=d?d.to.original:e,k=h.arr(f)?f[0]:k,w=L(h.arr(f)?f[1]:f,k),e=y(w)||y(k)||y(e);b.from=O(k,e);b.to=O(w,e);b.start=d?d.end:a.offset;b.end=b.start+b.delay+b.duration;b.easing=ca(b.easing);b.elasticity=(1E3-Math.min(Math.max(b.elasticity,1),999))/
1E3;b.isPath=h.pth(f);b.isColor=h.col(b.from.original);b.isColor&&(b.round=1);return d=b})}function ea(a,c){return r(p(a.map(function(a){return c.map(function(b){var c=J(a.target,b.name);if(c){var d=da(b,a);b={type:c,property:b.name,animatable:a,tweens:d,duration:d[d.length-1].end,delay:d[0].delay}}else b=void 0;return b})})),function(a){return!h.und(a)})}function R(a,c,d,b){var f="delay"===a;return c.length?(f?Math.min:Math.max).apply(Math,c.map(function(b){return b[a]})):f?b.delay:d.offset+b.delay+
b.duration}function fa(a){var c=D(ga,a),d=D(S,a),b=Z(a.targets),f=[],e=z(c,d),k;for(k in a)e.hasOwnProperty(k)||"targets"===k||f.push({name:k,offset:e.offset,tweens:aa(a[k],d)});a=ea(b,f);return z(c,{children:[],animatables:b,animations:a,duration:R("duration",a,c,d),delay:R("delay",a,c,d)})}function q(a){function c(){return window.Promise&&new Promise(function(a){return p=a})}function d(a){return g.reversed?g.duration-a:a}function b(a){for(var b=0,c={},d=g.animations,f=d.length;b<f;){var e=d[b],
k=e.animatable,h=e.tweens,n=h.length-1,l=h[n];n&&(l=r(h,function(b){return a<b.end})[0]||l);for(var h=Math.min(Math.max(a-l.start-l.delay,0),l.duration)/l.duration,w=isNaN(h)?1:l.easing(h,l.elasticity),h=l.to.strings,p=l.round,n=[],m=void 0,m=l.to.numbers.length,t=0;t<m;t++){var x=void 0,x=l.to.numbers[t],q=l.from.numbers[t],x=l.isPath?Y(l.value,w*x):q+w*(x-q);p&&(l.isColor&&2<t||(x=Math.round(x*p)/p));n.push(x)}if(l=h.length)for(m=h[0],w=0;w<l;w++)p=h[w+1],t=n[w],isNaN(t)||(m=p?m+(t+p):m+(t+" "));
else m=n[0];ha[e.type](k.target,e.property,m,c,k.id);e.currentValue=m;b++}if(b=Object.keys(c).length)for(d=0;d<b;d++)H||(H=E(document.body,"transform")?"transform":"-webkit-transform"),g.animatables[d].target.style[H]=c[d].join(" ");g.currentTime=a;g.progress=a/g.duration*100}function f(a){if(g[a])g[a](g)}function e(){g.remaining&&!0!==g.remaining&&g.remaining--}function k(a){var k=g.duration,n=g.offset,w=n+g.delay,r=g.currentTime,x=g.reversed,q=d(a);if(g.children.length){var u=g.children,v=u.length;
if(q>=g.currentTime)for(var G=0;G<v;G++)u[G].seek(q);else for(;v--;)u[v].seek(q)}if(q>=w||!k)g.began||(g.began=!0,f("begin")),f("run");if(q>n&&q<k)b(q);else if(q<=n&&0!==r&&(b(0),x&&e()),q>=k&&r!==k||!k)b(k),x||e();f("update");a>=k&&(g.remaining?(t=h,"alternate"===g.direction&&(g.reversed=!g.reversed)):(g.pause(),g.completed||(g.completed=!0,f("complete"),"Promise"in window&&(p(),m=c()))),l=0)}a=void 0===a?{}:a;var h,t,l=0,p=null,m=c(),g=fa(a);g.reset=function(){var a=g.direction,c=g.loop;g.currentTime=
0;g.progress=0;g.paused=!0;g.began=!1;g.completed=!1;g.reversed="reverse"===a;g.remaining="alternate"===a&&1===c?2:c;b(0);for(a=g.children.length;a--;)g.children[a].reset()};g.tick=function(a){h=a;t||(t=h);k((l+h-t)*q.speed)};g.seek=function(a){k(d(a))};g.pause=function(){var a=v.indexOf(g);-1<a&&v.splice(a,1);g.paused=!0};g.play=function(){g.paused&&(g.paused=!1,t=0,l=d(g.currentTime),v.push(g),B||ia())};g.reverse=function(){g.reversed=!g.reversed;t=0;l=d(g.currentTime)};g.restart=function(){g.pause();
g.reset();g.play()};g.finished=m;g.reset();g.autoplay&&g.play();return g}var ga={update:void 0,begin:void 0,run:void 0,complete:void 0,loop:1,direction:"normal",autoplay:!0,offset:0},S={duration:1E3,delay:0,easing:"easeOutElastic",elasticity:500,round:0},W="translateX translateY translateZ rotate rotateX rotateY rotateZ scale scaleX scaleY scaleZ skewX skewY perspective".split(" "),H,h={arr:function(a){return Array.isArray(a)},obj:function(a){return-1<Object.prototype.toString.call(a).indexOf("Object")},
pth:function(a){return h.obj(a)&&a.hasOwnProperty("totalLength")},svg:function(a){return a instanceof SVGElement},dom:function(a){return a.nodeType||h.svg(a)},str:function(a){return"string"===typeof a},fnc:function(a){return"function"===typeof a},und:function(a){return"undefined"===typeof a},hex:function(a){return/(^#[0-9A-F]{6}$)|(^#[0-9A-F]{3}$)/i.test(a)},rgb:function(a){return/^rgb/.test(a)},hsl:function(a){return/^hsl/.test(a)},col:function(a){return h.hex(a)||h.rgb(a)||h.hsl(a)}},A=function(){function a(a,
d,b){return(((1-3*b+3*d)*a+(3*b-6*d))*a+3*d)*a}return function(c,d,b,f){if(0<=c&&1>=c&&0<=b&&1>=b){var e=new Float32Array(11);if(c!==d||b!==f)for(var k=0;11>k;++k)e[k]=a(.1*k,c,b);return function(k){if(c===d&&b===f)return k;if(0===k)return 0;if(1===k)return 1;for(var h=0,l=1;10!==l&&e[l]<=k;++l)h+=.1;--l;var l=h+(k-e[l])/(e[l+1]-e[l])*.1,n=3*(1-3*b+3*c)*l*l+2*(3*b-6*c)*l+3*c;if(.001<=n){for(h=0;4>h;++h){n=3*(1-3*b+3*c)*l*l+2*(3*b-6*c)*l+3*c;if(0===n)break;var m=a(l,c,b)-k,l=l-m/n}k=l}else if(0===
n)k=l;else{var l=h,h=h+.1,g=0;do m=l+(h-l)/2,n=a(m,c,b)-k,0<n?h=m:l=m;while(1e-7<Math.abs(n)&&10>++g);k=m}return a(k,d,f)}}}}(),Q=function(){function a(a,b){return 0===a||1===a?a:-Math.pow(2,10*(a-1))*Math.sin(2*(a-1-b/(2*Math.PI)*Math.asin(1))*Math.PI/b)}var c="Quad Cubic Quart Quint Sine Expo Circ Back Elastic".split(" "),d={In:[[.55,.085,.68,.53],[.55,.055,.675,.19],[.895,.03,.685,.22],[.755,.05,.855,.06],[.47,0,.745,.715],[.95,.05,.795,.035],[.6,.04,.98,.335],[.6,-.28,.735,.045],a],Out:[[.25,
.46,.45,.94],[.215,.61,.355,1],[.165,.84,.44,1],[.23,1,.32,1],[.39,.575,.565,1],[.19,1,.22,1],[.075,.82,.165,1],[.175,.885,.32,1.275],function(b,c){return 1-a(1-b,c)}],InOut:[[.455,.03,.515,.955],[.645,.045,.355,1],[.77,0,.175,1],[.86,0,.07,1],[.445,.05,.55,.95],[1,0,0,1],[.785,.135,.15,.86],[.68,-.55,.265,1.55],function(b,c){return.5>b?a(2*b,c)/2:1-a(-2*b+2,c)/2}]},b={linear:A(.25,.25,.75,.75)},f={},e;for(e in d)f.type=e,d[f.type].forEach(function(a){return function(d,f){b["ease"+a.type+c[f]]=h.fnc(d)?
d:A.apply($jscomp$this,d)}}(f)),f={type:f.type};return b}(),ha={css:function(a,c,d){return a.style[c]=d},attribute:function(a,c,d){return a.setAttribute(c,d)},object:function(a,c,d){return a[c]=d},transform:function(a,c,d,b,f){b[f]||(b[f]=[]);b[f].push(c+"("+d+")")}},v=[],B=0,ia=function(){function a(){B=requestAnimationFrame(c)}function c(c){var b=v.length;if(b){for(var d=0;d<b;)v[d]&&v[d].tick(c),d++;a()}else cancelAnimationFrame(B),B=0}return a}();q.version="2.2.0";q.speed=1;q.running=v;q.remove=
function(a){a=P(a);for(var c=v.length;c--;)for(var d=v[c],b=d.animations,f=b.length;f--;)u(a,b[f].animatable.target)&&(b.splice(f,1),b.length||d.pause())};q.getValue=K;q.path=function(a,c){var d=h.str(a)?e(a)[0]:a,b=c||100;return function(a){return{el:d,property:a,totalLength:N(d)*(b/100)}}};q.setDashoffset=function(a){var c=N(a);a.setAttribute("stroke-dasharray",c);return c};q.bezier=A;q.easings=Q;q.timeline=function(a){var c=q(a);c.pause();c.duration=0;c.add=function(d){c.children.forEach(function(a){a.began=
!0;a.completed=!0});m(d).forEach(function(b){var d=z(b,D(S,a||{}));d.targets=d.targets||a.targets;b=c.duration;var e=d.offset;d.autoplay=!1;d.direction=c.direction;d.offset=h.und(e)?b:L(e,b);c.began=!0;c.completed=!0;c.seek(d.offset);d=q(d);d.began=!0;d.completed=!0;d.duration>b&&(c.duration=d.duration);c.children.push(d)});c.seek(0);c.reset();c.autoplay&&c.restart();return c};return c};q.random=function(a,c){return Math.floor(Math.random()*(c-a+1))+a};return q});

function updateCoords(e) {
    pointerX = (e.clientX || e.touches[0].clientX) - canvasEl.getBoundingClientRect().left,
    pointerY = e.clientY || e.touches[0].clientY - canvasEl.getBoundingClientRect().top
}
function setParticuleDirection(e) {
    var t = anime.random(0, 360) * Math.PI / 180
      , a = anime.random(50, 180)
      , n = [-1, 1][anime.random(0, 1)] * a;
    return {
        x: e.x + n * Math.cos(t),
        y: e.y + n * Math.sin(t)
    }
}
function createParticule(e, t) {
    var a = {};
    return a.x = e,
    a.y = t,
    a.color = colors[anime.random(0, colors.length - 1)],
    a.radius = anime.random(16, 32),
    a.endPos = setParticuleDirection(a),
    a.draw = function() {
        ctx.beginPath(),
        ctx.arc(a.x, a.y, a.radius, 0, 2 * Math.PI, !0),
        ctx.fillStyle = a.color,
        ctx.fill()
    }
    ,
    a
}
function createCircle(e, t) {
    var a = {};
    return a.x = e,
    a.y = t,
    a.color = "#F00",
    a.radius = .1,
    a.alpha = .5,
    a.lineWidth = 6,
    a.draw = function() {
        ctx.globalAlpha = a.alpha,
        ctx.beginPath(),
        ctx.arc(a.x, a.y, a.radius, 0, 2 * Math.PI, !0),
        ctx.lineWidth = a.lineWidth,
        ctx.strokeStyle = a.color,
        ctx.stroke(),
        ctx.globalAlpha = 1
    }
    ,
    a
}
function renderParticule(e) {
    for (var t = 0; t < e.animatables.length; t++)
        e.animatables[t].target.draw()
}
function animateParticules(e, t) {
    for (var a = createCircle(e, t), n = [], i = 0; i < numberOfParticules; i++)
        n.push(createParticule(e, t));
    anime.timeline().add({
        targets: n,
        x: function(e) {
            return e.endPos.x
        },
        y: function(e) {
            return e.endPos.y
        },
        radius: .1,
        duration: anime.random(1200, 1800),
        easing: "easeOutExpo",
        update: renderParticule
    }).add({
        targets: a,
        radius: anime.random(80, 160),
        lineWidth: 0,
        alpha: {
            value: 0,
            easing: "linear",
            duration: anime.random(600, 800)
        },
        duration: anime.random(1200, 1800),
        easing: "easeOutExpo",
        update: renderParticule,
        offset: 0
    })
}
function debounce(fn, delay) {
  var timer
  return function () {
    var context = this
    var args = arguments
    clearTimeout(timer)
    timer = setTimeout(function () {
      fn.apply(context, args)
    }, delay)
  }
}

var canvasEl = document.querySelector(".fireworks");
if (canvasEl) {
    var ctx = canvasEl.getContext("2d")
      , numberOfParticules = 30
      , pointerX = 0
      , pointerY = 0
      , tap = "mousedown"
      , colors = ["#FF1461", "#18FF92", "#5A87FF", "#FBF38C"]
      , setCanvasSize = debounce(function() {
        canvasEl.width = 2 * window.innerWidth,
        canvasEl.height = 2 * window.innerHeight,
        canvasEl.style.width = window.innerWidth + "px",
        canvasEl.style.height = window.innerHeight + "px",
        canvasEl.getContext("2d").scale(2, 2)
    },500)
      , render = anime({
        duration: 1 / 0,
        update: function() {
            ctx.clearRect(0, 0, canvasEl.width, canvasEl.height)
        }
    });
    document.addEventListener(tap, function(e) {
        "sidebar" !== e.target.id && "toggle-sidebar" !== e.target.id && "A" !== e.target.nodeName && "IMG" !== e.target.nodeName && (render.play(),
        updateCoords(e),
        animateParticules(pointerX, pointerY))
    }, !1),
    setCanvasSize(),
    window.addEventListener("resize", setCanvasSize, !1)
}
</script>
```

#### E.雪花特效

```

<script>
/*样式一*/
(function($){
	$.fn.snow = function(options){
	var $flake = $('<div id="snowbox" />').css({'position': 'absolute','z-index':'9999', 'top': '-50px'}).html('&#10052;'),
	documentHeight 	= $(document).height(),
	documentWidth	= $(document).width(),
	defaults = {
		minSize		: 10,
		maxSize		: 20,
		newOn		: 1000,
		flakeColor	: "#AFDAEF" /* 此处可以定义雪花颜色，若要白色可以改为#FFFFFF */
	},
	options	= $.extend({}, defaults, options);
	var interval= setInterval( function(){
	var startPositionLeft = Math.random() * documentWidth - 100,
	startOpacity = 0.5 + Math.random(),
	sizeFlake = options.minSize + Math.random() * options.maxSize,
	endPositionTop = documentHeight - 200,
	endPositionLeft = startPositionLeft - 500 + Math.random() * 500,
	durationFall = documentHeight * 10 + Math.random() * 5000;
	$flake.clone().appendTo('body').css({
		left: startPositionLeft,
		opacity: startOpacity,
		'font-size': sizeFlake,
		color: options.flakeColor
	}).animate({
		top: endPositionTop,
		left: endPositionLeft,
		opacity: 0.2
	},durationFall,'linear',function(){
		$(this).remove()
	});
	}, options.newOn);
    };
})(jQuery);
$(function(){
    $.fn.snow({ 
	    minSize: 5, /* 定义雪花最小尺寸 */
	    maxSize: 50,/* 定义雪花最大尺寸 */
	    newOn: 300  /* 定义密集程度，数字越小越密集 */
    });
});
</script>

<script>
/*样式二*/
/* 控制下雪 */
function snowFall(snow) {
    /* 可配置属性 */
    snow = snow || {};
    this.maxFlake = snow.maxFlake || 200;   /* 最多片数 */
    this.flakeSize = snow.flakeSize || 10;  /* 雪花形状 */
    this.fallSpeed = snow.fallSpeed || 1;   /* 坠落速度 */
}
/* 兼容写法 */
requestAnimationFrame = window.requestAnimationFrame ||
    window.mozRequestAnimationFrame ||
    window.webkitRequestAnimationFrame ||
    window.msRequestAnimationFrame ||
    window.oRequestAnimationFrame ||
    function(callback) { setTimeout(callback, 1000 / 60); };

cancelAnimationFrame = window.cancelAnimationFrame ||
    window.mozCancelAnimationFrame ||
    window.webkitCancelAnimationFrame ||
    window.msCancelAnimationFrame ||
	window.oCancelAnimationFrame;
/* 开始下雪 */
snowFall.prototype.start = function(){
    /* 创建画布 */
    snowCanvas.apply(this);
    /* 创建雪花形状 */
    createFlakes.apply(this);
    /* 画雪 */
    drawSnow.apply(this)
}
/* 创建画布 */
function snowCanvas() {
    /* 添加Dom结点 */
    var snowcanvas = document.createElement("canvas");
    snowcanvas.id = "snowfall";
    snowcanvas.width = window.innerWidth;
    snowcanvas.height = document.body.clientHeight;
    snowcanvas.setAttribute("style", "position:absolute; top: 0; left: 0; z-index: 1; pointer-events: none;");
    document.getElementsByTagName("body")[0].appendChild(snowcanvas);
    this.canvas = snowcanvas;
    this.ctx = snowcanvas.getContext("2d");
    /* 窗口大小改变的处理 */
    window.onresize = function() {
        snowcanvas.width = window.innerWidth;
        /* snowcanvas.height = window.innerHeight */
    }
}
/* 雪运动对象 */
function flakeMove(canvasWidth, canvasHeight, flakeSize, fallSpeed) {
    this.x = Math.floor(Math.random() * canvasWidth);   /* x坐标 */
    this.y = Math.floor(Math.random() * canvasHeight);  /* y坐标 */
    this.size = Math.random() * flakeSize + 2;          /* 形状 */
    this.maxSize = flakeSize;                           /* 最大形状 */
    this.speed = Math.random() * 1 + fallSpeed;         /* 坠落速度 */
    this.fallSpeed = fallSpeed;                         /* 坠落速度 */
    this.velY = this.speed;                             /* Y方向速度 */
    this.velX = 0;                                      /* X方向速度 */
    this.stepSize = Math.random() / 30;                 /* 步长 */
    this.step = 0                                       /* 步数 */
}
flakeMove.prototype.update = function() {
    var x = this.x,
        y = this.y;
    /* 左右摆动(余弦) */
    this.velX *= 0.98;
    if (this.velY <= this.speed) {
        this.velY = this.speed
    }
    this.velX += Math.cos(this.step += .05) * this.stepSize;

    this.y += this.velY;
    this.x += this.velX;
    /* 飞出边界的处理 */
    if (this.x >= canvas.width || this.x <= 0 || this.y >= canvas.height || this.y <= 0) {
        this.reset(canvas.width, canvas.height)
    }
};
/* 飞出边界-放置最顶端继续坠落 */
flakeMove.prototype.reset = function(width, height) {
    this.x = Math.floor(Math.random() * width);
    this.y = 0;
    this.size = Math.random() * this.maxSize + 2;
    this.speed = Math.random() * 1 + this.fallSpeed;
    this.velY = this.speed;
    this.velX = 0;
};
// 渲染雪花-随机形状（此处可修改雪花颜色！！！）
flakeMove.prototype.render = function(ctx) {
    var snowFlake = ctx.createRadialGradient(this.x, this.y, 0, this.x, this.y, this.size);
    snowFlake.addColorStop(0, "rgba(255, 255, 255, 0.9)");  /* 此处是雪花颜色，默认是白色 */
    snowFlake.addColorStop(.5, "rgba(255, 255, 255, 0.5)"); /* 若要改为其他颜色，请自行查 */
    snowFlake.addColorStop(1, "rgba(255, 255, 255, 0)");    /* 找16进制的RGB 颜色代码。 */
    ctx.save();
    ctx.fillStyle = snowFlake;
    ctx.beginPath();
    ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
    ctx.fill();
    ctx.restore();
};
/* 创建雪花-定义形状 */
function createFlakes() {
    var maxFlake = this.maxFlake,
        flakes = this.flakes = [],
        canvas = this.canvas;
    for (var i = 0; i < maxFlake; i++) {
        flakes.push(new flakeMove(canvas.width, canvas.height, this.flakeSize, this.fallSpeed))
    }
}
/* 画雪 */
function drawSnow() {
    var maxFlake = this.maxFlake,
        flakes = this.flakes;
    ctx = this.ctx, canvas = this.canvas, that = this;
    /* 清空雪花 */
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    for (var e = 0; e < maxFlake; e++) {
        flakes[e].update();
        flakes[e].render(ctx);
    }
    /*  一帧一帧的画 */
    this.loop = requestAnimationFrame(function() {
        drawSnow.apply(that);
    });
}
/* 调用及控制方法 */
var snow = new snowFall({maxFlake:60});
snow.start();
</script>
```

## 五、添加网站运行时间

```
<span id="timeDate">载入天数...</span><span id="times">载入时分秒...</span>
<script>
    var now = new Date(); 
    function createtime() { 
        var grt= new Date("08/10/2018 17:38:00");//在此处修改你的建站时间，格式：月/日/年 时:分:秒
        now.setTime(now.getTime()+250); 
        days = (now - grt ) / 1000 / 60 / 60 / 24; dnum = Math.floor(days); 
        hours = (now - grt ) / 1000 / 60 / 60 - (24 * dnum); hnum = Math.floor(hours); 
        if(String(hnum).length ==1 ){hnum = "0" + hnum;} minutes = (now - grt ) / 1000 /60 - (24 * 60 * dnum) - (60 * hnum); 
        mnum = Math.floor(minutes); if(String(mnum).length ==1 ){mnum = "0" + mnum;} 
        seconds = (now - grt ) / 1000 - (24 * 60 * 60 * dnum) - (60 * 60 * hnum) - (60 * mnum); 
        snum = Math.round(seconds); if(String(snum).length ==1 ){snum = "0" + snum;} 
        document.getElementById("timeDate").innerHTML = "本站已安全运行 "+dnum+" 天 "; 
        document.getElementById("times").innerHTML = hnum + " 小时 " + mnum + " 分 " + snum + " 秒"; 
    } 
setInterval("createtime()",250);
</script>
```

## 六、添加相册

### Hexo+Github实现相册功能

- 最终效果请看这里：http://lawlite.me/photos/

#### 一、说明

##### 1、关于

- 我使用的主题是[hexo-theme-yilia](https://github.com/litten/hexo-theme-yilia)，其中实现相册功能的方案是同步`instagram`上面的图片，但是现在`instagram`被禁，不能使用了
- 下面是通过自己的方式实现了相册功能，其中的**样式**还是使用该主题提供的

##### 2、方案

- 在`github`上**新建一个仓库**，主要用于存储图片，可以通过`url`访问到，也方便管理
- 将要放到相册的图片处理成`json`格式的数据，然后进行访问，这里`json`的格式需要配合要使用的样式，所以需要处理成**特定格式**的`json`数据，下面会给出
- **图片裁剪**，因为相册显示的样式最好是**正方形**的的图片，这里使用脚本处理一下
- **图片压缩**，相册显示的图片是压缩后的图片，提高加载的速度，打开后的图片是原图。

#### 二、实现

##### 1、github操作

- 建立一个用于存储相册的仓库，我这里fork为`Blog-Back-Up_bak`的仓库修改为Blog-Back-Up https://github.com/JiangJiaWei520/Blog-Back-Up_bak.git
  ![这里写图片描述](D:\OneDrive - shjd\GitHub\hexo_notes\themes\tree\source\images\20170413212532950)
- 关于`git`的命令行操作和配置不再给出

##### 2、博客操作

- 在**博客**目录的`source`文件夹下建立一个`photos`文件夹

- 将样式文件放到`photos`文件夹下，样式文件我都放到了`github`上：https://github.com/lawlite19/Blog-Back-Up/tree/master/blog_photos_copy

  ```
   assets/empty.png
   data.json
   index.ejs
   index.md
   ins.css
   ins.js
   lazyload.min.js
  ```

      var minSrc = 'https://raw.githubusercontent.com/JiangJiaWei520/Blog-Back-Up/master/photos/' + data.link[i];
      var src = 'https://raw.githubusercontent.com/JiangJiaWei520/Blog-Back-Up/master/photos/' + data.link[i];

- 修改index.md

  ```
  ---
  layout: post
  slug: "photos"
  title: "相册"
  noDate: "true"
  comments: "false"
  ---
  <link rel="stylesheet" href="./ins.css">
  
  <div class="photos-btn-wrap">
  	<a class="photos-btn active" href="javascript:void(0)">Photos</a>
  	<a class="photos-btn" href="#">待续</a>
  </div>
  <div class="instagram itemscope">
  	<a href="https://bk.jiang7zzz.xyz/" target="_blank" class="open-ins">图片正在加载中…</a>
  </div>
  <script>
    (function() {
      var loadScript = function(path) {
        var $script = document.createElement('script')
        document.getElementsByTagName('body')[0].appendChild($script)
        $script.setAttribute('src', path)
      }
      setTimeout(function() {
        loadScript('./ins.js')
      }, 0)
    })()
  </script>
  ```

  

- 修改ins.js文件，主要是里面的render函数

  - 其中的`url`对应到你的`github`放图片的地址


```stylus
    var render = function render(res) {
      var ulTmpl = "";
      for (var j = 0, len2 = res.list.length; j < len2; j++) {
        var data = res.list[j].arr;
        var liTmpl = "";
        for (var i = 0, len = data.link.length; i < len; i++) {
          var minSrc = 'https://raw.githubusercontent.com/lawlite19/blog-back-up/master/min_photos/' + data.link[i];
          var src = 'https://raw.githubusercontent.com/lawlite19/blog-back-up/master/photos/' + data.link[i];
          var type = data.type[i];
          var target = src + (type === 'video' ? '.mp4' : '.jpg');
          src += '';

          liTmpl += '<figure class="thumb" itemprop="associatedMedia" itemscope="" itemtype="http://schema.org/ImageObject">\
                <a href="' + src + '" itemprop="contentUrl" data-size="1080x1080" data-type="' + type + '" data-target="' + src + '">\
                  <img class="reward-img" data-type="' + type + '" data-src="' + minSrc + '" src="/assets/img/empty.png" itemprop="thumbnail" onload="lzld(this)">\
                </a>\
                <figcaption style="display:none" itemprop="caption description">' + data.text[i] + '</figcaption>\
            </figure>';
        }
        ulTmpl = ulTmpl + '<section class="archives album"><h1 class="year">' + data.year + '年<em>' + data.month + '月</em></h1>\
        <ul class="img-box-ul">' + liTmpl + '</ul>\
        </section>';
      }
```

##### 3、图片处理

- **python脚本文件**都放在了这里：https://github.com/lawlite19/Blog-Back-Up

- 修改tool.py

  ```
     指向博客地址-更新data.json
     with open("../person_blog/source/photos/data.json","w") as fp:
  ```

###### (1) 裁剪图片

- 去图片的中间部分，裁剪为**正方形**
- 对应的裁剪函数

```stylus
    def cut_by_ratio(self):  
        """按照图片长宽进行分割
        
        ------------
        取中间的部分，裁剪成正方形
        """  
        im = Image.open(self.infile)  
        (x, y) = im.size  
        if x > y:  
            region = (int(x/2-y/2), 0, int(x/2+y/2), y)  
        elif x < y:  
            region = (0, int(y/2-x/2), x, int(y/2+x/2))  
        else:  
            region = (0, 0, x, y)  

        #裁切图片  
        crop_img = im.crop(region)  
        #保存裁切后的图片  
        crop_img.save(self.outfile) 
```

###### (2) 压缩图片

- 把图片进行压缩，方便相册的加载

```stylus
def compress(choose, des_dir, src_dir, file_list):
    """压缩算法，img.thumbnail对图片进行压缩，
    
    参数
    -----------
    choose: str
            选择压缩的比例，有4个选项，越大压缩后的图片越小
    """
    if choose == '1':
        scale = SIZE_normal
    if choose == '2':
        scale = SIZE_small
    if choose == '3':
        scale = SIZE_more_small
    if choose == '4':
        scale = SIZE_more_small_small
    for infile in file_list:
        img = Image.open(src_dir+infile)
        # size_of_file = os.path.getsize(infile)
        w, h = img.size
        img.thumbnail((int(w/scale), int(h/scale)))
        img.save(des_dir + infile)
```

##### 4、github提交

- 处理完成之后需要将处理后的图片提交到`github`上
- 这里同样使用脚本的方式，需要将`git`命令行配置到环境变量中

```stylus
def git_operation():
    '''
    git 命令行函数，将仓库提交
    
    ----------
    需要安装git命令行工具，并且添加到环境变量中
    '''
    os.system('git add --all')
    os.system('git commit -m "add photos"')
    os.system('git push origin master')
```

##### 5、json数据处理

- 下面就需要将图片信息处理成`json`数据格式了，这里为重点

- 最终需要的json格式的数据如下图：
  ![这里写图片描述](D:\OneDrive - shjd\GitHub\hexo_notes\themes\tree\source\images\20170413212556724)

- 这里我采用的方式是读取

  图片的名字

  作为其中的

  text

  的内容，图片的命名如下图

  - 最前面是日期，然后用`_`进行分隔
  - 后面是图片的描述信息，注意不要包含`_`和`.`符号
    ![这里写图片描述](D:\OneDrive - shjd\GitHub\hexo_notes\themes\tree\source\images\20170413212609912)

- 实现代码：

  - 注意代码中`../lawlite19.github.io/source/photos/data.json`是对应到我的博客的路径，这里根据需要改成自己博客的路径

```stylus
def handle_photo():
    '''根据图片的文件名处理成需要的json格式的数据
    
    -----------
    最后将data.json文件存到博客的source/photos文件夹下
    '''
    src_dir, des_dir = "photos/", "min_photos/"
    file_list = list_img_file(src_dir)
    list_info = []
    for i in range(len(file_list)):
        filename = file_list[i]
        date_str, info = filename.split("_")
        info, _ = info.split(".")
        date = datetime.strptime(date_str, "%Y-%m-%d")
        year_month = date_str[0:7]            
        if i == 0:  # 处理第一个文件
            new_dict = {"date": year_month, "arr":{'year': date.year,
                                                                   'month': date.month,
                                                                   'link': [filename],
                                                                   'text': [info],
                                                                   'type': ['image']
                                                                   }
                                        } 
            list_info.append(new_dict)
        elif year_month != list_info[-1]['date']:  # 不是最后的一个日期，就新建一个dict
            new_dict = {"date": year_month, "arr":{'year': date.year,
                                                   'month': date.month,
                                                   'link': [filename],
                                                   'text': [info],
                                                   'type': ['image']
                                                   }
                        }
            list_info.append(new_dict)
        else:  # 同一个日期
            list_info[-1]['arr']['link'].append(filename)
            list_info[-1]['arr']['text'].append(info)
            list_info[-1]['arr']['type'].append('image')
    list_info.reverse()  # 翻转
    final_dict = {"list": list_info}
    with open("../lawlite19.github.io/source/photos/data.json","w") as fp:
        json.dump(final_dict, fp)
```

#### 三、其他

- 你可以根据需要进行修改`python`脚本代码，这里一些细节可能处理的不好
- 留言板：http://lawlite.me/留言板/
- 效果展示
  - 相册
    ![这里写图片描述](D:\OneDrive - shjd\GitHub\hexo_notes\themes\tree\source\images\20170413212626654)
  - 留言板
    ![这里写图片描述](D:\OneDrive - shjd\GitHub\hexo_notes\themes\tree\source\images\20170413212637100)
- 一些问题有人总结了，请查看：https://blog.csdn.net/wardseptember/article/details/82780684
  或者是我博客下的留言：http://lawlite.me/2017/04/13/Hexo-Github实现相册功能/

