# Rocket

express-GraphQL server and React example to interface the SpaceX API.

## Getting Started

Just clone and npm install.  

```
$ npm run server
```

### GraphQL query examples (URL: localhost:5000/graphql)

All Flights

```
{
  launches {
    flight_number,
    mission_name,
    launch_year,
    launch_success,
    launch_data_local,
    rocket {
      rocket_id,
      rocket_name,
      rocket_type
    }
  }
}

```

Find A Flight

```
{
  launch(flight_number: 2) {
    flight_number,
    mission_name,
    launch_year,
    launch_success,
    launch_data_local,
    rocket {
      rocket_id,
      rocket_name,
      rocket_type
    }
  }
}

```

```
{
  rockets {
    rocket_id,
    rocket_name,
    rocket_type
  }
}
```