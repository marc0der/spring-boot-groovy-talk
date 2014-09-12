####Spring Boot

#####Components

###Application

```
	@EnableAutoConfiguration
	@ComponentScan("zim")
	class Application {
	    static void main(String[] args){
	        new SpringApplication(Application).run(args)
	    }
	}
```
