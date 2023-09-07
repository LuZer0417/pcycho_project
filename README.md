# pcycho_project
实现了简单的微博关键字爬虫+基于GPT 3.5模型的情感分析

## 1 微博爬虫

## 1.1 思路
微博爬虫跟一般网页的爬虫思路不太一样，尤其是涉及到“关键字”查询功能的时候，就不能是简单的把网页上的文字爬取下来

step1:选择手机端网页作为爬取目标，该网址防爬虫不强，打开手机端页面
* 微博手机端
https://m.weibo.cn/

step2:在微博搜索框随便搜一个关键字，然后进入开发者模式（F12），再刷新界面

step3:我们想爬取的内容就在，“getindex”里面，说明我们如果能够从本地访问“getindex”里面内容的话，我们通过正则表达式就可以提取我们想要的内容

tips: geiIndex里面的内容是以json的格式存在的

step3:找标头(Request header)

step4: 找到User-Agent，它也在Request header下面

step5: 找到请求url和参数

## 1.2 代码执行前加入参数

（1）想搜索的关键字

（2）替换掉标头(Request header)

（3）直接运行



















