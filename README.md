## About

This is an example project that illustrates creating a RESTful API in Spring Boot along with OAuth2 security implementation using h2 DB.
Related blog post: https://gigsterous.github.io/engineering/2017/03/01/spring-boot-4.html
Imported and ran the app on 10th October 2018 and is working.

## Runnning this project

```
mvn spring-boot:run
```

## Get token

```
curl -X POST --user 'gigy:secret' -d 'grant_type=password&username=peter@example.com&password=password' http://localhost:8000/gigy/oauth/token
```

## Example commands

Getting all people from the API:
```
curl -i -H "Accept: application/json" -H "Content-Type: application/json" -H "Authorization: Bearer $TOKEN" -X GET http://localhost:8000/gigy/people
```

## LICENSE

The code is released under the Apache License 2.0. See LICENSE for details.
