## 文档地址
>第五篇：https://testerhome.com/topics/18142  
>第四篇：https://testerhome.com/topics/15657   
>第三篇：https://testerhome.com/topics/15352  
>第二篇：https://testerhome.com/topics/14801   
>第一篇：https://testerhome.com/topics/13269  
>其余篇：https://tech.kujiale.com/zi-yan-jie-kou-ce-shi-ping-tai/  
>使用者操作记录：
http://note.youdao.com/noteshare?id=06f2a9c75079a4e317d9f8bed25429fb&sub=6BA79F3EEE854AF2BAEE45902B2D0FCB  
## ChangeLog
>### 2.2.5  
>1.模块页面下一页按钮缺失  
>2.接口、用例、任务名全部支持中文，并加上正则限制        
>3.readme.md文件加下ChangeLog    
>### 2.2.4  
>1.新增requirements文件  
>2.支持单用例调试和查看报告  
>3.任务表修改，将任务名和uuid拆开  
>4.环境配置里新增https选择  
>5.邮件能够在里面描述下本次测试是哪个环境，哪些接口，执行情况等概要信息  
>6.接口页面如果某个值显示超过25个字段，显示25个字段+...,hover可见  
>7.去除用例页面优先级筛选和删除列表用例文件字段  
>8.用例页面新增生效中sql和nosql数，点击带参数跳转sql和nosql列表页  

>### 2.2.3
>1.接口名首字母不允许为数字  
>2.接口查询请求发了两次  
>3.修复编辑接口数据呈现  

>### 2.2.2
>1.新增生效中用例数，点击带上该行用例名跳转到用例页面  
>2.sql可以按照数据库名称搜索  
>3.优化接口名、用例名支持中文，后端限制不支持全数字，防止执行用例时造成白屏问题  
>4.添加的容易填错信息的placeholder引导  
>5.修改前端框架引用，提升性能  
>6.将页面中引入移至页面外引用,jquery代码移动到pageDeal文件，去除冗余代码  
>7.修复执行任务造成的数据权限混乱的问题  
>8.生成脚本加上了接口无用例的校验，防止执行用例时造成白屏问题  

>###2.2.1
>1.执行状态由前端触发  
>2.执行任务由原先的同步任务变更成异步线程完成  
>3.hotfix接口页面和函数模块  

>### 2.2.0
>1.新增redis操作  
>2.新增接口测试过程中自定义函数方法的定义和引入  
>3.对于不同项目组的数据隔离  
>4.改写单测执行的报告和首页数据展示报告的样式  
>5.admin后台对于用户，项目，模块功能的开发  
>6.在生成的unittest插桩，监控脚本执行进度，执行任务实时进度  
>7.断言开发小工具可以直接解析jsonpath，支持4种方式断言：字典、jsonpath、返回状态码、数据库sql查询出的变量解析  
>8.新增put和delete方法  

>### 2.1.3
>1.表carrytask变更，新增字段htmlreport，successlogname，errorlogname，修改request/models.py,需要进行数据库迁移  
>2.修改request/views.py,public/run,py,requestnew/urls.py,templates/main/task.html,新增static/img/backgrounds/noreport.png图片,task/textreport.html和task/nohtmlreport.html文件,新增web端的日志识别  
>3.修改templates/main/report.html，修改了报告样式bug  
>4.修改requestnew/setting.py的TEMPLATES对象的59行变更为'DIRS': [os.path.join(BASE_DIR, 'templates'),os.path.join(BASE_DIR, 'task')]  

>### 2.1.2
>1.新增mongo和mysql索引（索引放置群文件）  
>2.修改request/view.py文件，修改项目名和用例对不上的问题  
>3.修改template/main/report.html,颜色部分，断言错误fail采用红色，系统错误error采用黄色  
>4.新增public/ExtentHTMLTestRunner.py,修改public/run.py和spider.py,集成新版的单次报告，修改爬虫部分  
>5.修改public/view.py,public/make_testcase.py和task/template文件,将用例和步骤备注信息和新版本报告绑定  

>### 2.1.1
>1.新增版本文件  
>2.修改public/make_testcase.py文件，优化生成脚本文件  
>3.修改template/case.py和template/step.py,对于用例名、步骤名、任务名正则限制，只允许0-9a-zA-Z_等字符  
>4.修改template/task.py，修改失败重跑限制，加入了0次限制(无需失败重跑)  


>### 2.1.0
>1.修改public/make_testcase.py文件，优化生成脚本文件  
>2.修改template/case.py和request/view.py,修复生成脚本时不能同时选中2个页面的脚本  


