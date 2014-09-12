####Spring Boot

###Build

```
buildscript {
    repositories {
        url "http://repo.spring.io/libs-release"
    }
    dependencies {
        classpath "org.springframework.boot:spring-boot-gradle-plugin:1.1.5.RELEASE"
    }
}
apply plugin: 'spring-boot'
apply plugin: 'groovy'
repositories {
    url 'http://repo.spring.io/release'
}
dependencies {
    compile "org.codehaus.groovy:groovy:2.3.7"
    compile "org.springframework.boot:spring-boot-starter-web"
    compile "org.springframework.boot:spring-boot-starter-actuator"
    compile "org.springframework.boot:spring-boot-starter-remote-shell"
    compile "org.springframework.boot:spring-boot-starter-data-mongodb"
}
```
`build.gradle`
