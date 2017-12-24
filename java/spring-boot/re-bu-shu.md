# Spring Boot 在开发过程中热部署

## Maven 添加依赖

```xml
            <dependency>  
                        <groupId>org.springframework.boot</groupId>  
                        <artifactId>spring-boot-devtools</artifactId>  
                        <optional>true</optional>  
            </dependency>  
```

## Maven 添加插件

```
<!--spring boot plugin start-->
    <plugins>
      <plugin>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-maven-plugin</artifactId>
        <!--配置热部署-->
        <dependencies>
          <dependency>
            <groupId>org.springframework</groupId>
            <artifactId>springloaded</artifactId>
            <version>1.2.0.RELEASE</version>
          </dependency>
        </dependencies>
      </plugin>
    </plugins>
    <!--spring boot plugin end-->
```