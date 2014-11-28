# Java 类库

目的：为 Java 服务器端及Android开发提供常见功能类库，提升开发效率。

## 结构（名称未定，暂以lib代替）

```
 /libworkspace
  |-/cn.gyyx.lib
  |-/cn.gyyx.lib.android
  |-/cn.gyyx.lib.android.v4
 ...
```

## 功能

> https://github.com/springside/springside4/wiki/Design

1. *Memcache 客户端*
	`Spymemcached`，`xmemcached`
2. *日志*
	`Slf4j` + `Logback`
3. 加解密：MD5/HMACSHA1/AES/DES/3DES/RSA
	`java.security`
4. 编码
	- URL
	- Base64：`commons-codec`
	- 16 进制
5. 时间戳
	`new Date().getTime()`/`System.currentTimeMills()`
6. 常见字符串处理
	`lang3`，`Guava`，`pinyin4j`
7. *配置*
	[PropertiesParser](https://github.com/fivesmallq/nihiler-common/blob/master/src/org/nihiler/common/PropertiesParser.java)
8. Annotation
9. 文件导入导出
	`Apache POI`
10. 验证码
	`kaptcha`
11. IP
12. Cookie（Spring和非Spring）
13. Web
	`HttpClient`（非Spring）
14. JSON/XML
	`Jackson`，`fastjson`/`JAXB`，`dom4j`
15. *`Guava`*
16. *`joda-time`*
17. `jsoup`

## 场景

1. 应用进程 java xxx.jar
	`Runtime.getRuntime().addShutdownHook(shutdownThread)` => `Runtime.getRuntime().halt(0)`

## 开发原则

1. 优先使用 Maven 引用成熟稳定第三方库
2. 提供简易使用方法的封装
