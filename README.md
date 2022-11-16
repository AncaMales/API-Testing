# API-Testing
In this repository are some API Testing that I realized in my self-taught studies. The tool that I used is Postman.

----
#### Weather Forecast API Testing
API request for weather forecast for 5 days with data every 3 hours by city name.

**API call**

api.openweathermap.org/data/2.5/forecast?q=***{city name},{state code},{country code}***&appid=***{API key}***

**Parameters**

- **q** is required and represents the city name

- **appid** is required and represents the unique API key (than can always be found on the personal account page under the "API key" tab on https://openweathermap.org/)

- **mode** is optional and represents the response format. JSON format is used by default.

- **cnt** is optional and represents the number of timestamps, which will be returned in the API response.

- **units** is optional and represents the units of measurement. standard, metric and imperial units are available.
- **lang** is optional and represents the language.

