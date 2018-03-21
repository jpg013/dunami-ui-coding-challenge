## Dunami UI Coding Challenge

##### Description
The goal of this challenge is to build a simple front-end application around a public rest api (https://swapi.co/). On load the app should request data from the following endpoint:
```
https://swapi.co/api/people/
```
and display a list item for each of  each of the people returned in the JSON repsonse. Each display list item should contain the following properties.
1. Name
2. Height
3. Gender
4. Birth Year
5. Name and Popluation of Home Planet

##### `Note`

The Home Planet name and population data do not come back in the /people payload, but rather you will get a url of a rest point that you will need to call to retrieve that data, e.g.

```
homeworld": "https://swapi.co/api/planets/1/,
```

##### Searching
In addition to display a list of the data, there should also be an input box to search people based on their name. The end user of the application should be able to enter in part of, or the entire name of a person in the star wars db and get retrieve the data for the matched search results. The SWAPI api allows for searching on each rest endpoint by doing the following

```
https://swapi.co/api/people/?search=luke,
```
Which will return the following result:

```
{
    "count": 1,
    "next": null,
    "previous": null,
    "results": [
        {
            "name": "Luke Skywalker",
            "height": "172",
            "mass": "77",
            "hair_color": "blond",
            "skin_color": "fair",
            "eye_color": "blue",
            "birth_year": "19BBY",
            "gender": "male",
            "homeworld": "https://swapi.co/api/planets/1/",
            "films": [
                "https://swapi.co/api/films/2/",
                "https://swapi.co/api/films/6/",
                "https://swapi.co/api/films/3/",
                "https://swapi.co/api/films/1/",
                "https://swapi.co/api/films/7/"
            ],
            "species": [
                "https://swapi.co/api/species/1/"
            ],
            "vehicles": [
                "https://swapi.co/api/vehicles/14/",
                "https://swapi.co/api/vehicles/30/"
            ],
            "starships": [
                "https://swapi.co/api/starships/12/",
                "https://swapi.co/api/starships/22/"
            ],
            "created": "2014-12-09T13:50:51.644000Z",
            "edited": "2014-12-20T21:17:56.891000Z",
            "url": "https://swapi.co/api/people/1/"
        }
    ]
}
```

##### Grading Criteria
Here are the main things we are looking for in your application:

1. Functionality: The application should work according to the criteria described above.
2. Code Quality: We aren't looking for anything fancy, but we want to see clear, maintainable, and consistent code.
3. User-Interface: How well the UI performs/functions for the end-user.
4. Creativity: This is a fairly open coding challenge in terms of requirements, we want you to show off your creativity.

Happy Coding!
