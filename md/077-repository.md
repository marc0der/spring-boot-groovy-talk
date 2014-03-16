####Spring Boot

#####Stereotypes

###Repository

```
@Repository
interface StuffRepository extends MongoRepository<Stuffing, BigInteger>{
	List<Stuffing> findByName(String name)
}
```
