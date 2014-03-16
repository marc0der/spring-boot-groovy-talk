####Spring Boot

#####Components

###Configuration

```
@Configuration
public class MongoConfiguration extends AbstractMongoConfiguration {

    String getDatabaseName() {
        "somedb"
    }

    Mongo mongo() throws Exception {
        new Mongo()
    }

    String getMappingBasePackage() {
        "my.package.model";
    }
}

```
