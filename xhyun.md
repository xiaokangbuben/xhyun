# 文章相关接口说明
测试域名：  http://139.199.189.241:8080/liaoliao/

### 1.获取首页多个menu的id跟名称，获取banner的图片  get  base/listByType/{type}.do
#### 请求参数
|参数        |必选   |类型    	|说明|
---         |---    |---    	|---|
type	    |true  |string       |类型 banner(首页banner位图片)，menu（主页menu）|


#### 响应参数类型说明
|参数        	|类型    	|说明|
|---         	|---    	|---|
|id              |int		|menuId|
|name           |String		|主页menu名称|



#### 响应数据
```
{
  "dataList": [
    {
      "code": 1,
      "validStatus": 1,
      "createTime": 1487257774000,
      "name": "产品中心",
      "id": 31,
      "type": "menu"
    },
    {
      "code": 2,
      "validStatus": 1,
      "createTime": 1487257775000,
      "name": "解决方案",
      "id": 32,
      "type": "menu"
    },
    {
      "code": 3,
      "validStatus": 1,
      "createTime": 1487257776000,
      "name": "服务项目",
      "id": 33,
      "type": "menu"
    },
    {
      "code": 4,
      "validStatus": 1,
      "createTime": 1487257777000,
      "name": "新闻中心",
      "id": 34,
      "type": "menu"
    },
    {
      "code": 5,
      "validStatus": 1,
      "createTime": 1487257778000,
      "name": "联系我们",
      "id": 35,
      "type": "menu"
    },
    {
      "code": 6,
      "validStatus": 1,
      "createTime": 1487257779000,
      "name": "关于我们",
      "id": 36,
      "type": "menu"
    }
  ],
  "status": "success"
}
```

------------

### 2.获取menuId获取类型  get  /type/getTypeList/{menuId}.do
#### 请求参数
|参数        |必选   |类型    	|说明|
---         |---    |---    	|---|
menuId	    |true  |int      | |


#### 响应参数类型说明
|参数        	|类型    	|说明|
|---         	|---    	|---|
|id              |int		|menuId|
|name           |String		|类型名称|

#### 响应数据
```
{
  "dataList": [
    {
      "validStatus": 1,
      "createTime": 1506236560000,
      "name": "净化器",
      "menuId": 31,
      "id": 1
    },
    {
      "validStatus": 1,
      "createTime": 1506236578000,
      "name": "过滤器",
      "menuId": 31,
      "id": 2
    }
  ],
  "status": "success"
}
```

------------

### 3.获取人物列表  get  /people/getPeopleList.do
#### 请求参数
|参数        |必选   |类型    	|说明|
---         |---    |---    	|---|



#### 响应参数类型说明
|参数        	|类型    	|说明|
|---         	|---    	|---|


#### 响应数据
```
{
  "dataList": [
    {
      "imgUrl": "http://d.5857.com/juxs_160516/001.jpg",
      "validStatus": 1,
      "createTime": 1506145211000,
      "name": "乔布斯",
      "id": 1,
      "detail": "纽约归国的高级商业精英，投资公司高管。高挑美丽、气质出众的冷美人。特立独行，精准如公式的言谈举止和海量的知识储备令人印象深刻。高智商低情商的代表，强悍的工作能力下，是纯真如婴儿的心。对数字极为敏感，逻辑思维强大，外表冷淡不好接触，实则怀揣身世之谜，随时活在怕自己发疯的高压之下，不敢与人多做接触，在爱情上更是白纸一张。归国本是为了寻找弟弟，却在身世之谜逐渐揭开的同时，意外地收获了友情与爱情……\r\n\r\n安迪寻找到自己患有精神病的弟弟，安迪连忙乖乖过去,想拉小明的手,可小明就像见瘟神,来不及地往秀媛身后躲。\r\n\r\n\r\n纽约归国的高级商业精英，投资公司高管。高挑美丽、气质出众的冷美人。特立独行，精准如公式的言谈举止和海量的知识储备令人印象深刻。高智商低情商的代表，强悍的工作能力下，是纯真如婴儿的心。对数字极为敏感，逻辑思维强大，外表冷淡不好接触，实则怀揣身世之谜，随时活在怕自己发疯的高压之下，不敢与人多做接触，在爱情上更是白纸一张。归国本是为了寻找弟弟，却在身世之谜逐渐揭开的同时，意外地收获了友情与爱情……\r\n\r\n安迪寻找到自己患有精神病的弟弟，安迪连忙乖乖过去,想拉小明的手,可小明就像见瘟神,来不及地往秀媛身后躲。",
      "job": "CTO"
    },
    {
      "imgUrl": "http://img.zybus.com/uploads/allimg/140523/1-140523155101.jpg",
      "validStatus": 1,
      "createTime": 1506231958000,
      "name": "刘文静",
      "id": 2,
      "detail": "纽约归国的高级商业精英，投资公司高管。高挑美丽、气质出众的冷美人。特立独行，精准如公式的言谈举止和海量的知识储备令人印象深刻。高智商低情商的代表，强悍的工作能力下，是纯真如婴儿的心。对数字极为敏感，逻辑思维强大，外表冷淡不好接触，实则怀揣身世之谜，随时活在怕自己发疯的高压之下，不敢与人多做接触，在爱情上更是白纸一张。归国本是为了寻找弟弟，却在身世之谜逐渐揭开的同时，意外地收获了友情与爱情……\r\n\r\n安迪寻找到自己患有精神病的弟弟，安迪连忙乖乖过去,想拉小明的手,可小明就像见瘟神,来不及地往秀媛身后躲。",
      "job": "COO"
    }
  ],
  "status": "success"
}
```

------------

### 4.获取menuId下的文章列表 分页  get  /article/getByMenu/{menuId}.do?page=1&pageSize=10
#### 请求参数
|参数        |必选   |类型    	|说明|
---         |---    |---    	|---|
|menuId	    |true  |int      | |
|page	    |true  |int      | |
|pageSize	    |true  |int      | |

#### 响应参数类型说明
|参数        	|类型    	|说明|
|---         	|---    	|---|
|id              |int		|文章id|
|title           |String		|文章标题|
|createTime          |long		|文章发布时间|
|imgUrl          |String		|文章图片地址|

#### 响应数据
```
{
  "total": 4,
  "dataList": [
    {
      "imgUrl": "http://wiki.mbalib.com/w/images/5/54/Steve_Jobs.jpg",
      "articeTypeId": 1,
      "validStatus": 1,
      "createTime": 1506232553000,
      "menuId": 31,
      "id": 1,
      "title": "1乔布斯传记"
    },
    {
      "imgUrl": "http://wiki.mbalib.com/w/images/5/54/Steve_Jobs.jpg",
      "articeTypeId": 1,
      "validStatus": 1,
      "createTime": 1506232553000,
      "menuId": 31,
      "id": 2,
      "title": "2乔布斯传记"
    },
    {
      "imgUrl": "http://wiki.mbalib.com/w/images/5/54/Steve_Jobs.jpg",
      "articeTypeId": 1,
      "validStatus": 1,
      "createTime": 1506232553000,
      "menuId": 31,
      "id": 3,
      "title": "3乔布斯传记"
    },
    {
      "imgUrl": "http://wiki.mbalib.com/w/images/5/54/Steve_Jobs.jpg",
      "articeTypeId": 1,
      "validStatus": 1,
      "createTime": 1506232553000,
      "menuId": 31,
      "id": 4,
      "title": "4乔布斯传记"
    }
  ],
  "status": "success"
}
```

### 5.获取articleTypeId下的文章列表 分页  get  /article/getByArticleType/{articleTypeId}.do?page=1&pageSize=10
#### 请求参数
|参数        |必选   |类型    	|说明|
---         |---    |---    	|---|
|articleTypeId	    |true  |int      | 分类id，跟上面articleTypeId相同|
|page	    |true  |int      | |
|pageSize	    |true  |int      | |

#### 响应参数类型说明
|参数        	|类型    	|说明|
|---         	|---    	|---|
|id              |int		|文章id|
|title           |String		|文章标题|
|createTime          |long		|文章发布时间|
|imgUrl          |String		|文章图片地址|

#### 响应数据
```
{
  "total": 4,
  "dataList": [
    {
      "imgUrl": "http://wiki.mbalib.com/w/images/5/54/Steve_Jobs.jpg",
      "articeTypeId": 1,
      "validStatus": 1,
      "createTime": 1506232553000,
      "menuId": 31,
      "id": 1,
      "title": "1乔布斯传记"
    },
    {
      "imgUrl": "http://wiki.mbalib.com/w/images/5/54/Steve_Jobs.jpg",
      "articeTypeId": 1,
      "validStatus": 1,
      "createTime": 1506232553000,
      "menuId": 31,
      "id": 2,
      "title": "2乔布斯传记"
    },
    {
      "imgUrl": "http://wiki.mbalib.com/w/images/5/54/Steve_Jobs.jpg",
      "articeTypeId": 1,
      "validStatus": 1,
      "createTime": 1506232553000,
      "menuId": 31,
      "id": 3,
      "title": "3乔布斯传记"
    },
    {
      "imgUrl": "http://wiki.mbalib.com/w/images/5/54/Steve_Jobs.jpg",
      "articeTypeId": 1,
      "validStatus": 1,
      "createTime": 1506232553000,
      "menuId": 31,
      "id": 4,
      "title": "4乔布斯传记"
    }
  ],
  "status": "success"
}
```

### 6.获取文章详情  get /article/getArticleDetail/{articleId}.do
#### 请求参数
|参数        |必选   |类型    	|说明|
---         |---    |---    	|---|
|articleId	    |true  |int      | 文章id|


#### 响应参数类型说明
|参数        	|类型    	|说明|
|---         	|---    	|---|
|id              |int		|文章id|
|title           |String		|文章标题|
|createTime          |long		|文章发布时间|
|detail          |String		|文章内容|

#### 响应数据
```
{
  "data": {
    "imgUrl": "http://wiki.mbalib.com/w/images/5/54/Steve_Jobs.jpg",
    "articeTypeId": 1,
    "validStatus": 1,
    "createTime": 1506232553000,
    "menuId": 31,
    "id": 1,
    "detail": "<h2>史蒂夫·乔布斯（Steve Jobs）简介<img src=\"/server/ueditor/upload/image/demo.jpg\" title=\"\" alt=\"demo.jpg\" width=\"237\" height=\"157\"/></h2><ul class=\" list-paddingleft-2\"><li><p>职位：美国苹果公司创始人、前CEO</p></li><li><p>出生年月：1955年2月24日</p></li><li><p>父母：在婴儿时期被保罗·乔布斯(Paul Jobs)和克拉拉·乔布斯(ClaraJobs)领养，前者为一家激光公司的机械师，后者为<a href=\"http://wiki.mbalib.com/wiki/%E4%BC%9A%E8%AE%A1%E5%B8%88\" title=\"会计师\">会计师</a>，两人均已过世。</p></li><li><p>教育程度：1972年毕业于加利福尼亚州洛斯阿图斯的Homestead高中，后入读俄勒冈州波特兰的里德学院，六个月后退学。</p></li><li><p>外貌：身材修长，喜穿牛仔裤、黑色套领毛衣和跑鞋。</p></li></ul><p>　　1976年，时年21岁的乔布斯和26岁的沃兹尼艾克成立了苹果电脑公司。乔布斯先后领导缔造了麦金塔计算机、ipad、iPod、iTunes Store、iPhone等诸多知名<a href=\"http://wiki.mbalib.com/wiki/%E6%95%B0%E5%AD%97%E4%BA%A7%E5%93%81\" title=\"数字产品\">数字产品</a>。</p><p>　　1985年，乔布斯获得了由<a href=\"http://wiki.mbalib.com/wiki/%E9%87%8C%E6%A0%B9\" title=\"里根\">里根</a>总统授予的国家级技术勋章；</p><p>　　1997年成为<a href=\"http://wiki.mbalib.com/wiki/%E3%80%8A%E6%97%B6%E4%BB%A3%E5%91%A8%E5%88%8A%E3%80%8B\" title=\"《时代周刊》\">《时代周刊》</a>的封面人物；</p><p>　　2007年，史蒂夫·乔布斯被<a href=\"http://wiki.mbalib.com/wiki/%E3%80%8A%E8%B4%A2%E5%AF%8C%E3%80%8B%E6%9D%82%E5%BF%97\" title=\"《财富》杂志\">《财富》杂志</a>评为了年度最伟大商人。</p><p>　　2009年被财富杂志评选为这十年美国最佳CEO，同年当选时代周刊年度风云人物之一。</p><p>　　北京时间2011年8月25日，苹果公司宣布史蒂夫·乔布斯(Steve Jobs)辞职，并立即生效，他的<a href=\"http://wiki.mbalib.com/wiki/%E8%81%8C%E4%BD%8D\" title=\"职位\">职位</a>由<a href=\"http://wiki.mbalib.com/wiki/%E8%92%82%E5%A7%86%C2%B7%E5%BA%93%E5%85%8B\" title=\"蒂姆·库克\">蒂姆·库克</a>(<a href=\"http://wiki.mbalib.com/wiki/Tim_Cook\" title=\"Tim Cook\">Tim Cook</a>)接任。同时苹果宣布任命史蒂夫·乔布斯为公司<a href=\"http://wiki.mbalib.com/wiki/%E8%91%A3%E4%BA%8B%E9%95%BF\" title=\"董事长\">董事长</a>，蒂姆·库克将担任<a href=\"http://wiki.mbalib.com/wiki/%E8%91%A3%E4%BA%8B\" title=\"董事\">董事</a>。<sup class=\"reference\"><a href=\"http://wiki.mbalib.com/wiki/%E5%8F%B2%E8%92%82%E5%A4%AB%C2%B7%E4%B9%94%E5%B8%83%E6%96%AF#_note-0\" title=\"\">[2]</a></sup></p><p>　　北京时间2011年10月6日消息，苹果董事会宣布前CEO乔布斯于当地时间10月5日逝世，终年56岁。</p><p>　　乔布斯（Steve Jobs）有一个永远无法摆脱的敌人：他自己。在天才、能言善辩、敏锐的“天使”乔布斯里面，还有另一个“恶魔”乔布斯：冷酷、孤僻、暴躁、傲慢、一意孤行。你没法只保留其中好的那个他，能做到的只是让坏的那个不要永远失控。</p><p>　　乔布斯的60年代反传统风格悄悄的成为今日酷的注解，一双穿旧跑步鞋，一件套头的深色线衣，一条磨旧的蓝色牛仔裤，一脸的黑白相间胡子碴儿，只有乔布斯敢于穿着这样的装束参加<a href=\"http://wiki.mbalib.com/wiki/%E5%95%86%E4%B8%9A%E6%B4%BB%E5%8A%A8\" title=\"商业活动\">商业活动</a>。</p><p>[<a href=\"http://wiki.mbalib.com/w/index.php?title=%E5%8F%B2%E8%92%82%E5%A4%AB%C2%B7%E4%B9%94%E5%B8%83%E6%96%AF&action=edit&section=2\" title=\"编辑段落: 年少时的反叛青年\">编辑</a>]</p><p><a class=\"headline\"></a></p><h2>年少时的反叛青年</h2><p>　　史蒂夫·乔布斯（Steve Jobs）是一个孤儿，出生在1955年的硅谷，养父母是典型的美国<a href=\"http://wiki.mbalib.com/wiki/%E8%93%9D%E9%A2%86\" title=\"蓝领\">蓝领</a>。他的中学老师对他的评价是“一个孤僻的学生，看待事物的角度很特别”。然而这个孤僻的青年，却很幸运地早早找到了人生的黄金搭档——史蒂夫·沃兹尼艾克（Steven\r\n \r\nWozniak）一个电脑天才。除了对电子的爱好，他们都酷爱恶作剧。沃兹尼艾克热衷于制作电子小产品，他设计了一种“蓝盒子”，插入电话可以让使用者免费打长途电话。和沃兹尼艾克玩票的电子发烧友心态不同，乔布斯敏锐地发现了这种“娱乐”工具的商机。他开始到处<a href=\"http://wiki.mbalib.com/wiki/%E6%8E%A8%E9%94%80\" title=\"推销\">推销</a>，每卖出一个附上一张手写卡片“全世界掌握在你手中”，这成了产品的保修卡。他们这项的违法的生意开展得红红火火。</p><p>　　1972年乔布斯高中毕业，“蓝盒子”的生意也停止了。他选择了俄勒冈州波特兰的里德学院。在这里他获得了极为宝贵的人生经验。他从一个学生宗教领袖那儿学到了如何推销观点，如何具有个人魅力，成为领导统帅等。那时的乔布斯留着长发，经常赤脚，看起来就像是反叛的60年代的产物。但是很快他就选择了退学。</p><p>　　1974年乔布斯加入<a href=\"http://wiki.mbalib.com/wiki/Atari%E5%85%AC%E5%8F%B8\" title=\"Atari公司\">Atari公司</a>设计电子游戏，工作几个月后，他攒了足够的钱，漂洋过海和一个大学同学到印度朝圣，结果发现他们要找的大师已经去世，在这个佛教发源国漫游了几个月后，他顿捂，爱迪生对世界的贡献似乎比佛教大师要多得多。</p><p>[<a href=\"http://wiki.mbalib.com/w/index.php?title=%E5%8F%B2%E8%92%82%E5%A4%AB%C2%B7%E4%B9%94%E5%B8%83%E6%96%AF&action=edit&section=3\" title=\"编辑段落: “苹果”诞生\">编辑</a>]</p><p><a class=\"headline\"></a></p><h2>“苹果”诞生</h2><p>　　同年秋天回到硅谷的乔布斯，开始参加沃兹尼艾克的自制电脑俱乐部，同时精神方面也找到了寄托，开始参禅修行。沃兹尼艾克是一个技术天才，他们在乔布斯妹妹的卧室里设计苹果Ⅰ电脑，并开始在车库里生产制造。当地的一个电子产品<a href=\"http://wiki.mbalib.com/wiki/%E9%9B%B6%E5%94%AE%E5%95%86\" title=\"零售商\">零售商</a>看了他们的机器之后，便订购了50台。成功仿佛比预想得还要迅速。他们<a href=\"http://wiki.mbalib.com/wiki/%E5%8F%98%E5%8D%96\" title=\"变卖\">变卖</a>了所有值钱的东西，凑齐1300美元开始了创业。乔布斯将新公司命名为苹果（Apple）。这一名字的来源众说不一，不过可能是乔布斯为了纪念那年他在苹果园修行的愉快经历。</p><p>　　1976年，乔布斯和沃兹尼艾克将苹果Ⅰ定价为666美元推向<a href=\"http://wiki.mbalib.com/wiki/%E5%B8%82%E5%9C%BA\" title=\"市场\">市场</a>。苹果Ⅰ是第一台只有一个主板的<a href=\"http://wiki.mbalib.com/wiki/%E4%B8%AA%E4%BA%BA%E7%94%B5%E8%84%91\" title=\"个人电脑\">个人电脑</a>。看起来苹果Ⅰ的销量成绩喜人，但也只是上百台而已。</p><p>　　1976年底还从未有厂家出售过个人电脑，不过乔布斯却对这一市场坚信不疑。他想扩大公司的规模，便向<a href=\"http://wiki.mbalib.com/wiki/Atari\" title=\"Atari\">Atari</a>老板求助，结果被介绍给<a href=\"http://wiki.mbalib.com/wiki/Intel\" title=\"Intel\">Intel</a>（英特尔）前市场经理迈克·马库拉（Mike Markkula）。后者投资了91000美元到苹果公司，拥有30%的<a href=\"http://wiki.mbalib.com/wiki/%E8%82%A1%E4%BB%BD\" title=\"股份\">股份</a>。乔布斯和沃兹尼艾克各占30%。</p><p>[<a href=\"http://wiki.mbalib.com/w/index.php?title=%E5%8F%B2%E8%92%82%E5%A4%AB%C2%B7%E4%B9%94%E5%B8%83%E6%96%AF&action=edit&section=4\" title=\"编辑段落: “苹果”获得腾飞\">编辑</a>]</p><p><a class=\"headline\"></a></p><h2>“苹果”获得腾飞</h2><p>　　第二年乔布斯和沃兹尼艾克设计了苹果Ⅱ,它定义了个人电脑的<a href=\"http://wiki.mbalib.com/wiki/%E6%A0%87%E5%87%86\" title=\"标准\">标准</a>：显示器，键盘，驱动器，主板插槽，电源机箱。沃兹尼艾克花了两周时间设计的软盘驱动器精妙绝伦，只有同类产品的四分之一大小，苹果Ⅱ的所有设计完全由沃兹尼艾克一个人完成，甚至连其中的Basic解释程序也是沃兹尼艾克编的。</p><p>　　沃兹尼艾克认为能卖出1000台苹果Ⅱ就不错了。乔布斯却不这么想，他力邀为Intel设计广告的麦肯尼（Mckenna）为苹果制订<a href=\"http://wiki.mbalib.com/wiki/%E5%B9%BF%E5%91%8A%E7%AD%96%E7%95%A5\" title=\"广告策略\">广告策略</a>。在乔布斯每天打三四通电话的诚意下麦肯尼终于被说动。他为苹果作出了两大贡献，一是创造了苹果的标志：一个被咬了一口的苹果，带有彩虹般的线条。二是在《花花公子》上刊登广告，他的策略是突破电子迷这个小市场，在全国一炮而红。“沃兹尼艾克设计了一台很棒的电脑”，麦肯尼说：“但如果没有乔布斯,那台机器可能被束之高阁无人过问，沃兹尼艾克很幸运，因为他的伙伴是一位传教士。”</p><p>　　1977年举行的西海岸电脑展示会上，苹果Ⅱ大获成功。苹果Ⅱ设立了个人电脑的标准，短短三年<a href=\"http://wiki.mbalib.com/wiki/%E9%94%80%E5%94%AE%E9%A2%9D\" title=\"销售额\">销售额</a>超过了一亿美元，1980年乔布斯担任苹果公司<a href=\"http://wiki.mbalib.com/wiki/%E8%91%A3%E4%BA%8B%E9%95%BF\" title=\"董事长\">董事长</a>，苹果<a href=\"http://wiki.mbalib.com/wiki/%E5%85%AC%E5%BC%80%E4%B8%8A%E5%B8%82\" title=\"公开上市\">公开上市</a>，第一天从22美元涨到29美元，苹果的市值达到了12亿美元，25岁的乔布斯成为了白手起家的亿万<a href=\"http://wiki.mbalib.com/wiki/%E5%AF%8C%E7%BF%81\" title=\"富翁\">富翁</a>，当然他不是唯一的，苹果上市当月产生了四个亿万富翁和40个以上的百万富翁，个人电脑飞速发展的时代来临了。从1978年到1983年，苹果公司每年平均增长150％。</p><p>[<a href=\"http://wiki.mbalib.com/w/index.php?title=%E5%8F%B2%E8%92%82%E5%A4%AB%C2%B7%E4%B9%94%E5%B8%83%E6%96%AF&action=edit&section=5\" title=\"编辑段落: “苹果”遭遇挑战\">编辑</a>]</p><p><a class=\"headline\"></a></p><h2>“苹果”遭遇挑战</h2><p>　　苹果Ⅱ的成功并没有让乔布斯感到多大的满足,毕竟那是沃兹尼艾克的杰作。1979年乔布斯参观了<a href=\"http://wiki.mbalib.com/wiki/%E6%96%BD%E4%B9%90%E5%85%AC%E5%8F%B8\" title=\"施乐公司\">施乐公司</a>的Palo Alto研究中心，他看到了对方的目标是研究如何使电脑易于使用，用户不必打一个字，只需通过图符,窗口，菜单，鼠标可以操作电脑，他认为这才是电脑发展史上革命性的突破。</p><p>　　乔布斯立刻决定要制造一台施乐型的电脑，而且性能还要更好，价格还要低。于是新电脑麦金托什（Macintosh）被列入了议程。然而相比苹果Ⅱ的50万美元的开发<a href=\"http://wiki.mbalib.com/wiki/%E8%B4%B9%E7%94%A8\" title=\"费用\">费用</a>，Macintosh的达到了8000万美元，大大超过了<a href=\"http://wiki.mbalib.com/wiki/%E9%A2%84%E7%AE%97\" title=\"预算\">预算</a>。</p><p>　　经历了辉煌的五年之后，苹果面临电脑业巨人<a href=\"http://wiki.mbalib.com/wiki/IBM\" title=\"IBM\">IBM</a>的挑战。后者在1981年8月推出了IBM的个人电脑，<a href=\"http://wiki.mbalib.com/wiki/%E5%B8%82%E5%9C%BA%E8%90%A5%E9%94%80\" title=\"市场营销\">市场营销</a>非常成功，PC(Personal Computer)很快家喻户晓。只花了两年时间，PC的<a href=\"http://wiki.mbalib.com/wiki/%E9%94%80%E5%94%AE%E9%A2%9D\" title=\"销售额\">销售额</a>就超过了苹果，为了对抗IBM的强大<a href=\"http://wiki.mbalib.com/wiki/%E5%B8%82%E5%9C%BA%E7%AB%9E%E4%BA%89\" title=\"市场竞争\">市场竞争</a>，乔布斯向<a href=\"http://wiki.mbalib.com/wiki/%E7%99%BE%E4%BA%8B%E5%8F%AF%E4%B9%90\" title=\"百事可乐\">百事可乐</a>的总裁<a href=\"http://wiki.mbalib.com/w/index.php?title=%E7%BA%A6%E7%BF%B0%C2%B7%E6%96%AF%E5%8D%A1%E5%88%A9&action=edit\" class=\"new\" title=\"约翰·斯卡利\">约翰·斯卡利</a>(John·Scully)发出了邀约：“如果你留在百事可乐，五年后你只不过多卖了一些糖水给小孩，但到苹果，你可以改变整个世界”。</p><p>　　1984年，苹果公司出资百万美元在第10届橄榄球超级杯赛插播了一个引起极大争议的一分钟<a href=\"http://wiki.mbalib.com/wiki/%E7%94%B5%E8%A7%86%E5%B9%BF%E5%91%8A\" title=\"电视广告\">电视广告</a>，这个广告看起来更象是MV：走调的音乐，沉重的脚步声，成排剃光头的人一个接一个缓慢地走着，一张大脸（暗指IBM）正在屏幕上发表言论，一个年轻的女郎双手拿着铁槌冲进来，在屏幕前停下脚步，将铁槌向屏幕掷去，旋即发出震耳欲聋的粉碎声，旁白：“1月24号苹果公司将推出Macintosh电脑，你将了解为什么不同于奥威尔的《1984》。”奥威尔在《1984》这本畅销书里描述了像机械怪物似的电脑，而Macintosh正是要将电脑变成全世界千百万人的工具和玩具。</p><p>　　年末，苹果买下了《<a href=\"http://wiki.mbalib.com/wiki/%E6%96%B0%E9%97%BB%E5%91%A8%E5%88%8A\" title=\"新闻周刊\">新闻周刊</a>》选举特刊的所有广告版面，特刊的主题是：“民主的原则同样适用于技术，每人拥有一台电脑。”</p><p>　　Macintosh创造了奇迹，赢得媒体和狂热支持者的欢呼，乔布斯梦想Mactintosh能像电话击败电报一样获得划时代的胜利。</p><p>[<a href=\"http://wiki.mbalib.com/w/index.php?title=%E5%8F%B2%E8%92%82%E5%A4%AB%C2%B7%E4%B9%94%E5%B8%83%E6%96%AF&action=edit&section=6\" title=\"编辑段落: 乔布斯遭放逐\">编辑</a>]</p><p><a class=\"headline\"></a></p><h2>乔布斯遭放逐</h2><p>　　乔布斯设计Macintosh的初衷是想取代IBM在个人电脑市场的领先位置，因此采取了封闭式的设计结构，所有的外设都由苹果自主开发，配套软件跟不上，电子表格和文字处理软件两年后才推出。而且Macintosh在上市时测试还有很多问题，上市后整个开发队伍全都松懈了。这在很大程度上导致了Macintosh的<a href=\"http://wiki.mbalib.com/wiki/%E6%BB%9E%E9%94%80\" title=\"滞销\">滞销</a>。</p><p>　　乔布斯粗暴的工作作风也引起了开发者的不满，Macintosh的销量不断下滑，公司的<a href=\"http://wiki.mbalib.com/wiki/%E8%B4%A2%E6%94%BF%E8%B5%A4%E5%AD%97\" title=\"财政赤字\">财政赤字</a>到了无法忍受的地步。这个故步自封的错误是乔布斯败走麦城的开端，而将其推向深渊的却是他的盟友、苹果公司时任CEO斯卡利。斯卡利向董事会施压：如果乔布斯留在苹果，他就挂冠而去。在这个<a href=\"http://wiki.mbalib.com/wiki/%E5%85%B3%E9%94%AE%E6%97%B6%E5%88%BB\" title=\"关键时刻\">关键时刻</a>，<a href=\"http://wiki.mbalib.com/wiki/%E8%91%A3%E4%BA%8B%E4%BC%9A\" title=\"董事会\">董事会</a>选择了斯卡利。乔布斯被放逐了,他不再管理任何事务。</p><p>　　当年九月他向董事会递交了辞呈。当乔布斯向斯卡利递交了包括Mactionsh市场和技术骨干在内的想要带走的五个人名单时，董事会十分愤怒，授权斯卡利控告乔布斯非法使用苹果资料和技术，虽然最终达成和解，不过两者关系彻底破裂了。</p><p>　　乔布斯卖掉了他所有的苹果股票，只保留了一股，声称要得到<a href=\"http://wiki.mbalib.com/wiki/%E5%B9%B4%E5%BA%A6%E8%B4%A2%E5%8A%A1%E6%8A%A5%E5%91%8A\" title=\"年度财务报告\">年度财务报告</a>。他将这次分手作了浪漫的比喻：“我的心会一直留在那儿，和苹果公司的关系就像是初恋，我会永远眷恋苹果，就如同任何男士怀念他的初恋情人一样：缘尽情未了。”</p><p>[<a href=\"http://wiki.mbalib.com/w/index.php?title=%E5%8F%B2%E8%92%82%E5%A4%AB%C2%B7%E4%B9%94%E5%B8%83%E6%96%AF&action=edit&section=7\" title=\"编辑段落: “Next”——乔布斯的新方向\">编辑</a>]</p><p><a class=\"headline\"></a></p><h2>“Next”——乔布斯的新方向</h2><p>　　乔布斯创立了Next公司，为研究机构和学院提供专业配置的电脑，以加速研发的进程。在准备制造“下一代”电脑的同时，于1986年从《星球大战》的导演、光魔工业公司创办者乔治·卢卡斯那里收购来的动画技术公司<a href=\"http://wiki.mbalib.com/wiki/Pixar\" title=\"Pixar\">Pixar</a>（<a href=\"http://wiki.mbalib.com/wiki/%E7%9A%AE%E5%85%8B%E6%96%AF\" title=\"皮克斯\">皮克斯</a>）。乔布斯为苹果开创了桌面出版领域，下一步新领域是影象时代。但是事情远远不如他预想的那样顺理成章。Next电脑公司制作出来的电脑虽然看上去很美，但封闭的<a href=\"http://wiki.mbalib.com/wiki/%E7%B3%BB%E7%BB%9F\" title=\"系统\">系统</a>和昂贵的价格都让其无法成为电脑史上的下一个标准，却消耗了乔布斯几乎全部的精力与金钱，而皮克斯公司在十年间几乎没有丝毫建树。但是之后的事情却说明，面对失控的局面，他有多么强韧。</p><p>　　虽然经历了最初的挫折，乔布斯对Pixar和Next的坚持终于带来了丰硕的果实。1995年，Pixar和迪斯尼合作的《玩具总动员》在全球上映，票房收入达到4亿美元。Pixar借势<a href=\"http://wiki.mbalib.com/wi",
    "title": "1乔布斯传记"
  },
  "status": "success"
}
```

### 7.留言  post  /words/insert.do
#### 请求参数
|参数        |必选   |类型    	|说明|
---         |---    |---    	|---|
|name	    |true  |String      |名称|
|phone	    |true  |String      |手机号码 |
|comment	    |true  |string      | 留言内容|

#### 响应参数类型说明
|参数        	|类型    	|说明|
|---         	|---    	|---|


#### 响应数据
```
{
  "status": "success"
}
```