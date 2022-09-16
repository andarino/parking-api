## PARKING LOT
 API that can be used to control a parking   

![Spring](https://img.shields.io/badge/Spring-6DB33F?logo=spring&logoColor=white)
![JPA](https://img.shields.io/badge/Made%20with-JPA-brightgreen)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?logo=postgresql&logoColor=white)

API to control a condominium parking lot. Each condominium has a single place identified by the license plate, apartment and block.

## AUTHORIZATION
	(HttpMethod.GET, "/parking-spot/**").permitAll()
	(HttpMethod.POST, "/parking-spot").hasRole("USER")
	(HttpMethod.DELETE, "/parking-spot/**").hasRole("ADMIN")

## REQUEST

* BODY POST: 
```
{
	"parkingSpotNumber" : "188B",
	"licensePlateCar" : "AKC2316",
	"brandCar" : "Honda",
	"modelCar" : "hrv",
	"colorCar" : "branco",
	"responsibleName" : "joaozinho",
	"apartment" : "126",
	"block": "B"
}
```

