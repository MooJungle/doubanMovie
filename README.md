# movietrailer
douban movie

豆瓣电影网站实现
关键技术：
1、puppeteer爬取豆瓣电影网站热门电影200条、热门电视剧200条、正在上映电影50条并获取其电影名、海报地址、评分、豆瓣id等数据，并保存到mongoDB数据库。
2、通过数据库已有电影id和axios函数获取豆瓣电影官方api更多电影相关数据，包括电影上映日期、导演、演员、语言、片长、制片国家或地区等相关数据。
3、koa-router做后端路由。
4、art-template模板引擎实现组件封装和后端读取数据库后的数据渲染。



注：
豆瓣官方api可能于近两个月内由于某种原因已经停止开放，而之前保存在本地MongoDB数据库内的数据丢失。所以目前没有办法获得某部电影、电视剧的详情信息，但电影详情页保留了相关数据的渲染位置，期待豆瓣电影再次开放api平台。


待实现功能：
1、轮播图bug及翻页效果逻辑。
2、ajax实现标签选择数据。
3、懒加载。
4、影评。


注意：
1、下载项目：git clone https://github.com/MooJungle/cloudMusic.git
2、npm install下载相关依赖。
3、开启mongodb数据库，打开main.js1第13行注释，运行npm start爬虫，须修改task.js分别爬取热门电影、热门电视剧、正在上映的电影数据。
4、注释main.js第13行，开启第14行注释.运行npm start通过数据库中的数据在豆瓣电影api获取详细数据，须修改api.js完成电影电视剧正在上映的电影分别获取api数据。
5、注释main.js第14行，运行npm start预览效果。


部分界面展示：
![Image text](https://github.com/MooJungle/doubanMovie/blob/master/server/static/img/%E4%B8%BB%E9%A1%B51.jpg)；
![Image text](https://https://github.com/MooJungle/doubanMovie/blob/master/server/static/img/%E4%B8%BB%E9%A1%B52.jpg)；
![Image text](https://github.com/MooJungle/doubanMovie/blob/master/server/static/img/%E4%B8%BB%E9%A1%B53.jpg)；
![Image text](https://github.com/MooJungle/doubanMovie/blob/master/server/static/img/%E7%83%AD%E9%97%A8%E7%94%B5%E5%BD%B1.jpg)；
![Image text](https://github.com/MooJungle/doubanMovie/blob/master/server/static/img/%E7%83%AD%E9%97%A8%E7%94%B5%E8%A7%86%E5%89%A7.jpg)；
![Image text](https://github.com/MooJungle/doubanMovie/blob/master/server/static/img/%E7%94%B5%E5%BD%B1%E8%AF%A6%E6%83%85%E9%A1%B5.jpg)；


