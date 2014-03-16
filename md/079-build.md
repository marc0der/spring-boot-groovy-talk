####Spring Boot

###Build

```
buildscript {
    repositories {
        maven { url "http://repo.spring.io/libs-snapshot" }
    }
    dependencies {
        classpath "o..sf..boot:spring-boot-gradle-plugin:1.0.0.RC3"
    }
}
apply plugin: 'spring-boot'
repositories {
    maven { url 'http://repo.spring.io/milestone' }
}
dependencies {
    compile "org.codehaus.groovy:groovy:2.2.2"
    compile "org.springframework.boot:spring-boot-starter-web:1.0.0.RC4"
    compile "org.springframework.data:spring-data-commons:1.6.2.RELEASE"
}
```
`build.gradle`
