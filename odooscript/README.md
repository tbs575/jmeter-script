1、使用`Set User Email.jmx`脚本（配合set-mail.txt文件）来生成压测登陆账号
set-mail.txt文件定义用户登录的账号和密码 (User account file)

2、使用`Odoo_test.jmx`脚本（配合running-test.txt文件）来进行压力测试

running-test.txt文件文件定义说明：
账号名,密码,定义上传excel文件,循环导入excel多少次,是否执行到最后一步
循环导入excel多少次：将执行导入excel，试算科目余额多少次
是否执行到最后：表示该账户将执行到最后的月结、过账等操作

3、为每个测试账号准备需要导入凭证的文件，文件名在`running-test.txt`中定义

1、连接10.193.10.80:8567端口访问odoo
2、选择数据库oCaiGe - 01
