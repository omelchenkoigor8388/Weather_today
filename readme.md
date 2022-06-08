# Weather today 

### What is the program for?

**Weather today** is a graphical user interface that allows 
users to know the weather at any given time anywhere in 
the world.

### Functionality of the program

**Weather today** is a program that can give you 
accurate hydrometeorological information at any 
given time in any locality on our planet ... 
Using it you will be able to learn the following 
hydrometeorological data:
- Temperature
- Humidity
- Wind speed
- The situation in the sky (cloudy, cloudy, clear, etc.)

### How the program works

After entering your city in the search column
**Weather today** program takes up-to-date hydrometeorological
information from the site [https://openweathermap.org/](https://openweathermap.org/).
Then it will display the current information about the weather 
in a given city.

<img height="250" src="https://user-images.githubusercontent.com/106494942/172617976-273eb9f2-7a5d-4e74-a473-b9fcee33476c.jpg" width="250"/> <img height="250" src="https://user-images.githubusercontent.com/106494942/172618598-9a44d419-3b66-4cb4-b905-0ed56df1035a.jpg" width="250"/> <img height="250" src="https://user-images.githubusercontent.com/106494942/172618667-4306bb0c-bf90-47c5-ad71-28e243928b50.jpg" width="250"/>

### How to run the program?

1. To run the program you will need the installed programming 
    language PYTHON, if you do not have the latest version installed 
    go and install it [https://www.python.org/](https://www.python.org/).

2. To run the program you need to have your key from the open weather map.
   If you do not have it, go to the link and register 
   on the site[https://openweathermap.org/](https://openweathermap.org/).
   Then generate your unique API key.

   ![photo_2022-06-08_13-33-38](https://user-images.githubusercontent.com/106494942/172618724-62d48d9a-9915-46c8-b8e9-fbc186f8b358.jpg)

   ![photo_2022-06-08_13-33-41](https://user-images.githubusercontent.com/106494942/172618772-e04c1d85-eab5-45e9-81be-0d144bfc99da.jpg)

3. The API key must be inserted into the **Weather.py** file
```
    def weather(self, place):
        owm = OWM(' your unique API key') 
        mgr = owm.weather_manager()
        observation = mgr.weather_at_place(place)
        w = observation.weather
```
4. If all the above points have been passed, run the file **Weather.py**

### What was used to create the Weather today program?

- Python 3.9
- QT Designer(To create a graphic part of the program)
- Libraries :
    - PyQt5
    - pyowm
    - requests
- Site with hydro meteorological information https://openweathermap.org/
 
