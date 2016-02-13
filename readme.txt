单元测试：
Karma和Jasmine
集成测试：
Protractor，端到端测试，可以打开浏览器模拟用户的输入



前端框架管理器：bower
npm install -g bower

bower安装某个框架，默认会安装在bower_components下面

在使用linux命令touch .bowerrc，创建.bowerrc文件，在文件中指定路径：
{"directory": "app/public/lib"}

初始化前端框架：bower init

? description
? main file index.js
? what types of modules does this package expose?
? keywords node,express,bower,gulp,Karma,Jasmine,Protractor
? authors LemonYogurt
? license MIT
? homepage
? set currently installed components as dependencies? Yes
? add commonly ignored files to ignore list? Yes
? would you like to mark this package as private which prevents it from being accidentally published to the registry? (y
? would you like to mark this package as private which prevents it from being accidentally published to the registry? No

通过bower安装bootstrap和angularjs
bower install bootstrap --save
bower install angular angular-route --save


nodejs包管理器：npm
通过npm初始化node项目：npm init
初始化选项：
name: (netshop) netshop
version: (1.0.0)
description:
entry point: (index.js) index.js
test command: gulp test
git repository: https://github.com/LemonYogurt/netshop
keywords: node express bower gulp Karma Jasmine Protractor
author: LemonYogurt
license: (ISC) MIT

然后安装：
npm install express --save

推送到github上：
给项目添加一个忽略文件：.gitignore
**/lib
.idea
node_modules

git初始化项目：
git init
git add .
git commit -m "first commit"
git remote add origin https://github.com/LemonYogurt/netshop.git
git push -u origin master