# springboot 版本变化
2.2.*  serverTimezone=GMT%2B8  修改数据库连接时区设置，否则容易出现mysql数据库timestamp时间不准；
       测试类注解@RunWith(SpringRunner.class)@SpringBootTest替换为@SpringBootTest(webEnvironment = SpringBootTest.WebEnvironment.RANDOM_PORT)
2.3.*  pom手动增加 <dependency>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-starter-validation</artifactId>
               </dependency>
        依赖 ，否则validation不可用
