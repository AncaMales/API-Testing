# API-Testing
In this repository are some API Testing that I realized in my self-taught studies. The tool that I used is Postman.

----
#### Weather Forecast API Testing
API request for weather forecast for 5 days with data every 3 hours by city name.

**API call**

api.openweathermap.org/data/2.5/forecast?q=***{city name},{state code},{country code}***&appid=***{API key}***

**Parameters**

- **q** is required and represents the city name

- **appid** is required and represents the unique API key (it can always be found on the personal account page under the "API key" tab on https://openweathermap.org/)

- **mode** is optional and represents the response format. JSON format is used by default.

- **cnt** is optional and represents the number of timestamps, which will be returned in the API response.

- **units** is optional and represents the units of measurement. standard, metric and imperial units are available.
- **lang** is optional and represents the language.

![Get weather by city (units, lang)](https://user-images.githubusercontent.com/117184407/202178048-e5d5c7c3-903e-4a67-a83e-6d38e3c94d46.png)

---

#### CRUD operations testing

***Read*** using GET method
- read all the users from the database

**Parameters**
- **action** with the value **fetch_all** represents the parameter that gets all users

![Read](https://user-images.githubusercontent.com/117184407/202184538-4607ef5c-9b59-4483-8dd2-e38ce4b48b38.png)

***Create*** using POST method
- adding user with first name and last name

**Parameters**
- **insert** insert user
- **first_name** represents the first name
- **last_name** represents the last name
- 
![Create](https://user-images.githubusercontent.com/117184407/202192745-2bb3d27c-5e99-4436-afe2-b9986dcce595.png)

The result in the database:

![Create result](https://user-images.githubusercontent.com/117184407/202187648-bfccb3e3-1315-4b1d-b5ca-32fd92fff155.png)

***Update*** using POST method
- updating the user name

**Parameters**
- **id** the id of the user whose name it will be updated
- **first_name** represents the first name
- **last_name** represents the last name

![Update](https://user-images.githubusercontent.com/117184407/202188642-d5869ef2-9c50-4686-955c-8e39bf40ac54.png)

The result in the database:

![Update result](https://user-images.githubusercontent.com/117184407/202188909-44b679c8-357e-4265-b230-a9562587fd98.png)

***Delete*** using DELETE method
- deleting an user from the database

**Parameters**
- **action** with the value **delete**
- **id** the id of the user whose name it will be deleted, so the user "Margaret Thatcher" will be deleted.

![Delete](https://user-images.githubusercontent.com/117184407/202190477-a5a07d43-b8f0-4458-b2da-98c29854c726.png)
The result in the database:
![Delete result](https://user-images.githubusercontent.com/117184407/202190541-f16863d2-04c3-403b-a7b3-2983d6b0cf9c.png)

---

***OMDb API testing***
- The OMDb API is a RESTful web service to obtain movie information

**Parameters** for "Search movie by Title" action
- **apikey** represents the unique API key generated on https://www.omdbapi.com/ after the user creates an account
- **t** represents the title of the movie searched

![Search movie by title](https://user-images.githubusercontent.com/117184407/202195192-450eedf5-d91d-44e1-80e3-b8b187719d12.png)

**Parameters** for "Search movie by IMDb ID" action
- **apikey** represents the unique API key generated on https://www.omdbapi.com/ after the user creates an account
- **i** represents the title of the movie searched

![Search movie by ID](https://user-images.githubusercontent.com/117184407/202195433-f4272e38-5f43-4040-b130-f7bcb4b6eaed.png)

**Parameters** for "Search movie by Title/Type/Year/Plot/Data type" action
- **apikey** represents the unique API key generated on https://www.omdbapi.com/ after the user creates an account
- **t** represents the title of the movie searched
- **type** represents the type of the movie (movie, series, episode)
- **y** represents the year of release.
- **plot** returns short or full plot.
- **r** represents the the data type to return.

![Search movie by Title:Type:Year:Plot:Data type](https://user-images.githubusercontent.com/117184407/202196875-2bc083bf-ce5f-4a60-9d45-5f0d1235d256.png)

