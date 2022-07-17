## Hello and welcome to this coding challenge!

We would ask you to solve the following coding challenge in your preferred programming language. Some notes before starting:

- You can use the language and technology of your choice
- You can solve it the way you prefer, there is no perfect, but lots of good solutions
- No pressure time-wise, however it should not take too much time
- When you are done, ideally post in on github and send us the link. If that is not possible, simply send us back the project
- Have fun :-)

### Getting started

Given a list of destinations containing hotels with the following format (JSON):

```
[
    {
        mallorca: [
            {
                name: "Hotel Playa",
                stars: 3
            },
            {
                name: "Hotel Playa Deluxe",
                stars: 5
            }
        ],
        tyrol: [
            {
                name: "Hotel Mountain Budget",
                stars: 2
            },
            {
                name: "Hotel Mountain",
                stars: 3
            },
            {
                name: "Hotel Tyrol Deluxe",
                stars: 5
            }
        ]
    }
]
```

Your task is to create a program that takes one input parameter `stars` and returns a list of hotels filtered by their `stars` attribute. Additionally, there should be the `destination` attribute within each hotel (see example below).

The program can be a REST service, command line or any kind of frontend application (e.g. React).

### Example

If you choose to go with a REST service, it could contain one `/hotels` endpoint that returns all Hotels with the given `stars` query.

In other words, if you run it locally, e.g. on http://localhost:3000/hotels?stars=3, the service should return:

```
[
    {
        name: "Hotel Playa",
        stars: 3,
        destination: "Mallorca"
    },
    {
        name: "Hotel Mountain",
        stars: 3,
        destination: "Tyrol"
    }
]
```






