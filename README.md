# Real-time-Weather

A simple webpage the display current weather report of any city around the world.
The API send the data in JSON format similar to this
~~~~
Object
    base: "stations"
    clouds:
        all: 40
        __proto__: Object
    cod: 200
    coord:
        lat: 18.52
        lon: 73.86
        __proto__: Object
    dt: 1590640650
    id: 1259229
    main:
        feels_like: 303.22
        grnd_level: 949
        humidity: 34
        pressure: 1009
        sea_level: 1009
        temp: 306.34
        temp_max: 306.34
        temp_min: 306.34
        __proto__: Object
    name: "Pune"
    sys:
        country: "IN"
        sunrise: 1590625674
        sunset: 1590672970
        __proto__: Object
    timezone: 19800
    weather: Array(1)
        0:
            description: "scattered clouds"
            icon: "03d"
            id: 802
            main: "Clouds"
            __proto__: Object
        length: 1
        __proto__: Array(0)
    wind:
        deg: 290
        speed: 6.86
      __proto__: Object
      __proto__: Object

~~~~

API used: 
----
> api.openweathermap.org/data/2.5/weather?q={city name}&appid={your api key}

further modifications can be done by using other API from same source
* By city name
----
  > api.openweathermap.org/data/2.5/weather?q={city name},{state code}&appid={your api key}
  
  > api.openweathermap.org/data/2.5/weather?q={city name},{state code},{country code}&appid={your api key}
  
* By city Id
----
  > api.openweathermap.org/data/2.5/weather?id={city id}&appid={your api key}
 
* By geographic coordinates
----
  > api.openweathermap.org/data/2.5/weather?lat={lat}&lon={lon}&appid={your api key}
  
* By zip code
----
  > api.openweathermap.org/data/2.5/weather?zip={zip code},{country code}&appid={your api key}
  
API source:
----
https://openweathermap.org/
