####Spring Boot

#####Stereotypes

###Repository

```
	@Repository
	interface QuoteRepository extends MongoRepository<Quote, BigInteger> {
	    List<Quote> findByName(String name)
	}

```
