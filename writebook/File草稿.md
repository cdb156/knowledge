```
pom文件添加单元测试依赖：

[html] view plain copy 在CODE上查看代码片派生到我的代码片
<dependency>  
        <groupId>junit</groupId>  
        <artifactId>junit</artifactId>  
        <version>4.8.2</version>  
        <scope>test</scope>  
    </dependency>  

2 添加maven surefire插件依赖：
[html] view plain copy 在CODE上查看代码片派生到我的代码片
<plugin>  
            <groupId>org.apache.maven.plugins</groupId>  
            <artifactId>maven-surefire-plugin</artifactId>  
            <version>2.8</version>  
            <configuration>  
                <includes>  
                    <!--包含所有后缀为Test.jave的类 -->  
                    <include>**/*Test.java</include>  
                </includes>  
            </configuration>  
        </plugin>  

3 编写测试用例类，方法

4 命令行调用单元测试方法：

mvn test -Dtest=TestClassName#testMethod 
```
