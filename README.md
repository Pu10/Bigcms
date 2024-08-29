介绍
====

Bigcms是一个针对个人网站设计的微型内容管理系统。
![image](https://github.com/user-attachments/assets/f952c3f4-10dc-4627-ae72-9ed1ae39a6e0)

结构
====

```
mc-admin           后台
mc-files           内容
  |--theme         主题
  |--posts         文章
  |    |--data     数据
  |    |--index    索引
  |--pages         页面
       |--data     数据
       |--index    索引
```
       
URL格式
=======

文章: http://1.com/?post/[a-z0-5]{6}  
标签: http://1.com/?tag/[^/]+/  
页面: http://1.com/?([-a-zA-Z0-5]+/)+
 
模板标签
=======

```
mc_site_name()  // 网站标题  
mc_site_desc()  // 网站描述  
mc_user_nick()  // 站长昵称  

mc_theme_url() // 主题文件夹中文件的URL  

mc_next_post()   // 循环获取文章  
mc_the_name()    // 文章标题  
mc_the_date()    // 发布日期  
mc_the_time()    // 发布时间  
mc_the_content() // 文章内容  
mc_the_tags()    // 文章标签
```
