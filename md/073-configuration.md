####Spring Boot

#####Components

###Configuration

```
	@Configuration
	public class MongoConfiguration extends AbstractMongoConfiguration {

		String getDatabaseName() {
			"christmas"
		}

		Mongo mongo() throws Exception {
			new Mongo()
		}

		String getMappingBasePackage() {
			"christmas.package.stuff";
		}
	}
```
