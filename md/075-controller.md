####Spring Boot

#####Stereotypes

###Controller

```
	@Controller
	@RequestMapping("/festivity")
	class FestivityController {

		@Autowired
		StuffingRepository repository

		@Autowired
		TurkeyService service

		@RequestMapping("/party/{party}")
		@ResponseBody ResponseEntity party(@PathVariable String party){
			def stuffing = repository.findByName(party)
			def turkey = service.prepare(stuffing)
			new ResponseEntity(turkey, OK)
		}
	}

```

context: `/myapp/festivity/party/christmas`
