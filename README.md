"springmvcSimple" 

1-1简介
MVC核心思想：将业务数据抽取和业务数据呈现相互分离
MVC:Model-View-Controller
	Controller:控制层，调用业务逻辑产生数据Model
	Model:模型层，表示业务数据信息
	Controller：控制层，将产生的数据Model传递给视图层用来呈现
	View:视图层，呈现数据的UI
MVC是一种架构模式	
MVC是一种思考方式

1-2 Maven
  POM(Project Object Model)
  Dependency Management
  Coordinates 
坐标定位：
  <groupId>com.mvn</groupId>
  <artifactId>demoInstall</artifactId>
  <version>0.0.1-SNAPSHOT</version>
a.Spring MVC 安装:
    下载解压Maven
    配置环境变量 --> check: cmd mvn -version 
    配置Maven配置文件(本地仓库路径，镜像）
b.Eclipse配置maven
    选择本地解压的maven目录 Preferences-Maven->Installations   
    选择本地maven的配置文件 Preferences-Maven->User Settings	
c.Spring MVC项目搭建
    新建maven项目，选择webapp(注意eclipse会默认选择quickstart类型，此时需手动更改)
	查看JavaBuildPath缺省的folder，手动新建folder
	添加pom.xml中springmvc的依赖包
d.用Spring MVC进行开发
    配置web.xml文件
	新建一个controller类实现方法
	如果preferences没有web选项，就安装:install new software->http://download.eclipse.org/releases/juno->选择web and java ee development选项
	新建前端页面xxx.jsp 进行编辑
    在项目pom.xml文件目录下的cmd运行：mvn jetty:run
	当cmd窗口显示：[INFO] Started Jetty Server后就可以使用浏览器进行访问了:例如 http://localhost:8080/hello/mvc 
e.课程总结
    通过了springmvc实际运行结果

