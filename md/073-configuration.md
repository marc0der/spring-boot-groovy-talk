####Spring Boot

#####Components

###Configuration

```
	@Configuration
	class MongoConfiguration extends AbstractMongoConfiguration {

	    String getDatabaseName() {
	        "invasion"
	    }

	    Mongo mongo() throws Exception {
	        new MongoClient()
	    }
	}
```
