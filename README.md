# news-spider

#### 简介  
  本项目为基于node.js编写的爬虫项目(百度新闻)

#### 本地运行  
  ~~~bash
  node index.js    在本机 3001 端口上运行开发调试环境
  ~~~

#### 整体思路如下  

1. express启动一个简单的Http服务
2. 分析目标页面DOM结构，找到所要抓取的信息的相关DOM元素
3. 使用superagent请求目标页面
4. 动态页面（需要加载页面后运行JS或请求接口的页面）可以使用Nightmare模拟浏览器访问
5. 使用cheerio获取页面元素，获取目标数据

> 教程及文档 [分分钟教你用node.js写个爬虫](https://segmentfault.com/a/1190000014811373)
> 项目地址 [分分钟教你用node.js写个爬虫](https://segmentfault.com/a/1190000014811373)