# lightralab
基于Xml数据存储的实验室网站，可添加其它数据源的支持。


# updates

1.修改文件上传的名称策略：FileRenamePolicyPlugin
	在com.jfinal.upload包中新增FileRenamePolicyPlugin
	修改MultipartRequest第40行，调用FileRenamePolicyPlugin

2.表单数组上传：ToolModel
	在com.jfinal.core包中新增ToolModel类

3.增加sql打印格式化

	SqlReporter的55行，String info = "Sql: " + ToolSqlFormatter.format(String.valueOf(args[0]));

4.增加sql打印参数

	修改Dialect类，由于Oracle重写了打印方法，所以还修改了OracleDialect类

5.升级jetty9运行项目

	修改JettyServer类的88-99行
