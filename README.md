# movietrailer
douban movie

豆瓣电影网站实现
关键技术：
1、puppeteer爬取豆瓣电影网站热门电影200条、热门电视剧200条、正在上映电影50条并获取其电影名、海报地址、评分、豆瓣id等数据，并保存到mongoDB数据库。
2、通过数据库已有电影id和axios函数获取豆瓣电影官方api更多电影相关数据，包括电影上映日期、导演、演员、语言、片长、制片国家或地区等相关数据。
3、koa-router做后端路由。
4、art-template模板引擎实现组件封装和后端读取数据库后的数据渲染。





待实现功能：
1、轮播图bug及翻页效果逻辑。
2、ajax实现标签选择数据。
3、懒加载。
4、影评。


注意：
1、下载项目：git clone https://github.com/MooJungle/cloudMusic.git
2、npm install下载相关依赖。
3、开启mongodb数据库，打开main.js1第13行注释，运行npm start爬虫，须修修改task.js分别爬取热门电影、热门电视剧、正在上映的电影数据。
4、注释main.js第13行，开启第14行注释.运行npm start通过数据库中的数据在豆瓣电影api获取详细数据。
5、注释main.js第14行，运行npm start预览效果。