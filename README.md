# A blog for beginners named 'www.dreamylost.cn'  by  a java developer who comes from jxnu .
# feature1支才是最新的。 主分支废了 
## Branch1分支是我开发的项目完整版（add .提交），包含搜狐畅游评论，使用的话需要替换自己的appid,里面我只删除了CA证书，jar都在，用于测试。与feature1支不同的主要是修复分页的bug和评论是用的第三方插件
## 主要技术与说明  第一次写项目，考虑不周见谅。特别是图片缩略有问题  存在的问题都在笔记墙说了。本blog仅供新手学习.
### 1、JDK:1.8 (未使用1.8特性)<strong>修改->application-dev.properties, cmd-> java -jar blog.jar 即可运行项目 
### 注：本地不要使用java -jar运行最好，需要改为发布的服务器路径而且坑多，使用eclipse运行application.java最好，使用war则需要添加一 个转换和修改打包方方式具体百度。 主要需要修改配置如下：日志位置，索引位置，tomcat虚拟路径配置，sql url配置，https证书位置（我自 己的会删除，CA的，也可以自己用jdk工具生成，不再赘述） 均需要保证路径C:/web/uploads/存在（tomcat的虚拟路径，已经写死在代码中，默认在服务器与本机创建c:\web与uploads,linux按着改分隔符吧）在web里新建文件夹filenames,filenames存放静态资源file,则访问方式为ip:port/filenames/file,以此类推，注意Shiro拦截）
### 2、前端模板：来自国产开源框架Layui社区的分享“不落阁”，含百度分享等插件
### 3、全文检索：Lucene
### 4、前端模板引擎：Thymeleaf3.0（nekohtml）
### 5、字体：font-awesome
### 6、代码高亮：prettify
### 7、后台：SpringBoot1.5.8、Mybatis3.4.5、Mysql5.6
### 8、验证：jquery-validate、Shiro
### 9、日志：默认logback
### 10、单元测试：Junit4
### 11、数据库连接池：Druid(含sql与spring监控)
### 12、JSON工具 ：fastjson
### 13、web服务器:Tomcat8.5内嵌式 使用Https
### 14、发布方式：Jar
### 15、代码托管：github
### 16、依赖管理：maven
### 17、开发工具：MyEclipse2013 UE sublimetext
### 18、缓存：Myabtis二级缓存（友情链接）,redis缓存（验证码）,ehcache（权限）
### 主要功能，实体表，文章，文章分类，友情链接，点赞关系表，评论，留言。公告，博主信息表。多级评论暂未实现。
 
仅供参考 。【This is for your reference only.】
点个star更好  qaq 预览地址www.dreamylost.cn

 已使用 畅言插件代替文章评论模块。实现多级评论。感觉不太好所以该功能具体代码未更新。此处代码仍是自己写的需要审核的单级评论。
