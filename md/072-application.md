####Spring Boot

#####Components

###Application

```
@EnableAutoConfiguration
@ComponentScan("my.package")
class Application {
    static void main(String[] args){
        new SpringApplication(Application).run(args)
    }
}
```
