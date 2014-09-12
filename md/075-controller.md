####Spring Boot

#####Stereotypes

###Controller

```
	@Controller
	class InvasionController {

	    @Autowired
	    QuoteRepository repository

	    @RequestMapping("/invader/{name}")
	    @ResponseBody ResponseEntity quote(@PathVariable String name){
	        def quotes = repository.findByName(name)
	        if(!quotes) throw new InvaderNotFoundException(name)

	        def quote = quotes[(int)(Math.random() * quotes.size())]
	        new ResponseEntity(quote, OK)
	    }
	}

```

context: `/invader/zim`
