RSS 面前的 3 座大山
【找到 RSS 源】
【制作 RSS 源】
【维护 RSS 源】

【机密】内部资料之RSS 指导手册

## 指南之难

说起 RSS ，在很多年前我便听说，但旋即放弃，一是因为看到英文便没有了解的欲望，二是使用过程确实繁琐。

在这之后的又很多年，才在好奇的个性与折腾的习性之下，再次尝试，并使用至今。

就像年少是喜欢看各类探索、解密、异志、野史那样，用 RSS 可以订阅很多不见于主流媒体 / App，却又真实，有趣的内容。

极客、文青的博文，加精、置顶的帖子，专业、深度的期刊……

把这想看的一切，都汇于一处。

不仅了解他们想让你看到的，更要看看你想不到的！

将你探索世界的望远镜，握在手中。


### 找到 RSS 源

刚会用 RSS 时，很笨很无力：根本不知从哪找 RSS 源？

虽然知道只要找到页面上的那个屎黄色，像 wifi 信号一样的 RSS 图标……但这钛合金狗眼就是扫不到啊！

后来，咱又进化到了中级菜鸟，发现了一个“奥义”，直接在主域名后面加 feed 或者 rss 就可以（例如在 xxoo.com 后面加 feed，中间要打上 / ，也就是 xxoo.com/feed 即为 RSS 地址！）

像多数用 Wordpress 搭建的博客，后面加的是 feed 或者 rss 和 ?feed=rss 都可以。（想单独订阅其下的某个分类，也可以用这个方法。例如 YY 分类，就是 xxoo.com/category/yy/feed）

用 GitHub pages 搭建的 Hexo 博客则是加 atom.xml。

可是这个方法，也不是很通用，很多网站不提供 RSS 地址，你在后面加什么都没有用。就算提供了，也有可能加的是 feed.asp,feed.php,xx.rss 等奇葩的地址。

当然，现在这么原始的方法可以丢弃啦。还输啥域名 + feed ，直接上“一览插件”。遇到提供了 RSS 输出的网站，它的图标上会直接提示你，该站点提供了几个 RSS ，然后直接点订阅就可以了。

极客一点的同志也可以用“[油猴脚本](https://greasyfork.org/zh-CN/scripts/6261-rss-atom-feed-subscribe-button-generator)”，帮你找出当前网站的 RSS 地址。

还有是在不知道订阅啥的，也可以在一览的“[发现](http://www.yilan.io/explore/recommend/)”板块内，随便逛逛，或者用“[一览搜索](http://www.yilan.io/search)”找点感兴趣的。

不过，就像上面说得，网站不提供 RSS 输出，你找破了天也没用。还好，技术高，心肠好的程序猿很多。

热门如国内的微博，微信，知乎，国外的 Twitter, Facebook, Google+，都做了现成的 RSS。

例如，要订阅：

* 微博，用“[微博档案](http://sinacn.weibodangan.com)”

* 微信，用“[微广场](http://www.iwgc.cn)”（不知还能坚持多久，很多类似的都倒下了）

* 知乎，用“[一览](http://www.yilan.io/search)”

* 简书，用“[JianShu](http://jianshu.milkythinking.com)”（代码见 [GitHub](https://github.com/hutushen222/JianshuRSS)）

* 豆瓣一刻，请看该博主的“[文章](https://chi.miantiao.me/douban-yike-rss)”

* 知乎日报，又看该博主的“[文章](https://chi.miantiao.me/zhihu-daily-rss/)”

* 知乎专栏，再看该博主的“[文章](https://chi.miantiao.me/zhihuzhuanlan-rss/)”（目前失效，代码见 [GitHub](https://github.com/bpsk/zhihuzhuanlanRSS)）

* 知乎专栏，用“[lilydjwg](https://rss.lilydjwg.me/)”（代码见 [GitHub](https://github.com/lilydjwg/morerssplz)）

* 优酷，方法见百度

* 土豆，方法见百度

还有国外的：

* Twitter User，用“[TwitRSS](http://www.twitrss.me/)”或者国内用户利用他们提供的开源代码汉化的“[TPRSS](http://tprss.puteulanus.com/)”（代码见 [GitHub](https://github.com/ciderpunx/twitrssme)）

* [Morss](http://morss.it) 支持转全文，Twitter，DuckDuckGo 与 Bing 的搜索结果，Facebook，iTunes

* [Queryfeed](https://queryfeed.net) 提供 Twitter 用户和搜索结果，Google+ 的文章、图片，以及 Facebook

* [Exileed](http://feed.exileed.com/?lang=en) 提供 Facebook,Google+,Twitter


### 制作 RSS 源

虽然上面现成的 RSS 让你用的很开心，但毕竟覆盖面不广，程序猿也随时可能因为被妹子撩走了就不在维护了。

