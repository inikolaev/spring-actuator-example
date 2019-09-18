Spring Boot 2.0 Actuator Examples
=======================================

[Spring Actuator](https://spring.io/blog/2017/08/22/introducing-actuator-endpoints-in-spring-boot-2-0) 
with [Spring Boot 2.0](https://docs.spring.io/spring-boot/docs/current-SNAPSHOT/reference/htmlsingle/#production-ready-endpoints-custom) examples.

- Example of a Spring Boot Actuator

### Build
Execute the following command from the parent directory to build the jar file:
```
mvn clean install
```

### Run
From the parent directory, executte the following coommand to start the application:
```
java -jar target/spring-actuator-example-1.0.0.jar
```

You should notice the application starting up,
```
  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.8.RELEASE)

2019-09-18 21:34:55.641  INFO 28641 --- [           main] com.github.inikolaev.Application         : Starting Application on Zalando-09142 with PID 28641 (/Users/inikolaev/Projects/spring-actuator-example/target/spring-actuator-example-1.0.0.jar started by inikolaev in /Users/inikolaev/Projects/spring-actuator-example)
2019-09-18 21:34:55.648  INFO 28641 --- [           main] com.github.inikolaev.Application         : No active profile set, falling back to default profiles: default
2019-09-18 21:34:58.359  INFO 28641 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat initialized with port(s): 8080 (http)
2019-09-18 21:34:58.426  INFO 28641 --- [           main] o.apache.catalina.core.StandardService   : Starting service [Tomcat]
2019-09-18 21:34:58.427  INFO 28641 --- [           main] org.apache.catalina.core.StandardEngine  : Starting Servlet engine: [Apache Tomcat/9.0.24]
2019-09-18 21:34:58.653  INFO 28641 --- [           main] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring embedded WebApplicationContext
2019-09-18 21:34:58.653  INFO 28641 --- [           main] o.s.web.context.ContextLoader            : Root WebApplicationContext: initialization completed in 2804 ms
2019-09-18 21:34:59.745  INFO 28641 --- [           main] o.s.s.concurrent.ThreadPoolTaskExecutor  : Initializing ExecutorService 'applicationTaskExecutor'
2019-09-18 21:35:00.292  INFO 28641 --- [           main] o.s.b.a.e.web.EndpointLinksResolver      : Exposing 15 endpoint(s) beneath base path ''
2019-09-18 21:35:00.455  INFO 28641 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat started on port(s): 8080 (http) with context path ''
2019-09-18 21:35:00.468  INFO 28641 --- [           main] com.github.inikolaev.Application         : Started Application in 5.907 seconds (JVM running for 6.602)

```

Once the application starts up, navigate to `http://localhost:8080/actuator/health` in a browser, e.g., Chrome.
