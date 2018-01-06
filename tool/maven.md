# what is maven
 用来进行项目的构建。构建主要会遇到的问题：编译是找不到jar包，单元测试代码应该放在什么位置。

# how
1 统一开发规范与工具
2 统一管理 jar 包

https://ayayui.gitbooks.io/tutorialspoint-maven/content/book/maven_overview.html

##  build lifecycle

# 具体maven的使用
## pom文件结构 project object model


## mvn命令
mvn clean：清空输出目录（即 target 目录）
mvn compile：编译源代码
mvn package：生成构件包（一般为 jar 包或 war 包）
mvn install：将构件包安装到本地仓库
mvn deploy：将构件包部署到远程仓库
mvn dependency:tree   查看jar包的依赖来源
mvn clean install -Dmaven.test.skip=true  打jar包，并跳过测试



# 附件
简单的maven介绍：
https://my.oschina.net/huangyong/blog/194583
