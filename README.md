

## 注意！
* 本项目不是可运行项目，无需 clone 到本地，请直接运行脚本
* 本项目依赖于 Lombok 插件，请在 IDE 中安装 `Lombok Plugin`，了解 Lombok 请查看：[Lombok：让 Java 代码更优雅](https://mp.weixin.qq.com/s?__biz=MzI0OTIzOTMzMA==&mid=2247483851&idx=1&sn=007ceceaa3a3e6fecbeb23873a230e19&chksm=e995c386dee24a90c9493949bd1cb159114f5d457d4354a93050c3a218c5d111a193406dff74&mpshare=1&scene=1&srcid=0606I1Vkahdws6aFa04Ytvpv#rd)


## 前置条件
* [JDK 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
* [Maven 3](http://maven.apache.org/download.cgi)
* [Lombok](https://mp.weixin.qq.com/s?__biz=MzI0OTIzOTMzMA==&mid=2247483851&idx=1&sn=007ceceaa3a3e6fecbeb23873a230e19&chksm=e995c386dee24a90c9493949bd1cb159114f5d457d4354a93050c3a218c5d111a193406dff74&mpshare=1&scene=1&srcid=0606I1Vkahdws6aFa04Ytvpv#rd)


## 特点
* 基于 Spring Boot 1.5.9，内嵌 Jetty
* 提供全局异常捕获、View to Json、跨域访问等功能
* 提供 Maven Profile 和 Spring Profile 完美融合的解决方案
* 集成通用 Mapper 和 PageHelper，新增 BaseService，常用 CRUD 无需编写代码
* 集成 MyBatis Generator，额外提供功能强大的插件拓展 [MBG Plugin Extension](https://github.com/drtrang/mybatis-generator-extension)
* 集成 [Druid Spring Boot Starter](https://github.com/drtrang/druid-spring-boot)，无需显式声明数据源，支持多数据源
* 集成 Swagger2，HTTP 接口自动生成接口文档
* 集成常用工具，如 Copiers、CsvUtils、DateUtils……


```
mvn archetype:generate -DarchetypeGroupId=com.github.drtrang -DarchetypeArtifactId=maven-archetype-springboot -DarchetypeVersion=1.0.1 -DinteractiveMode=false -DarchetypeCatalog=local -DgroupId=${groupId} -DartifactId=${artifactId} -Dversion=${version} -Dpackage=${package}
```

### 启动项目
在项目的根路径下执行以下脚本：
```
mvn spring-boot:run
```

启动后即可通过浏览器访问该项目，默认端口号为 **8080**：
```html
http://localhost:8080

