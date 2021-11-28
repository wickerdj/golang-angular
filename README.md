# Golang & Angular

Following [Golang & Angular Series - Part 1: Developing and Securing Golang APIs](https://auth0.com/blog/developing-golang-and-angular-apps-part-1-backend-api/)

[Developing a To-Do List Application with Angular](https://auth0.com/blog/developing-golang-and-angular-apps-part-2-angular-front-end/)

## Progress

Made the code changes for Part 1. Need to test.

## Notes

## Manual testing

``` shell
# add a new to-do item
curl localhost:3000/todo -d '{"message": "finish writing the article"}'

# get all to-do items
curl localhost:3000/todo


# From the Auth0 site
## log in
## Go to API
## Find the test tab, copy the cURL command, the past into a terminal
## copy the access token and set it to environment variable
## So far I have only been able to get the API to return a 401 using the manual method

ACCESS_TOKEN="ey...Gg"

curl -H 'Authorization: Bearer '$ACCESS_TOKEN localhost:3000/todo -d '{"message": "finish writing the article"}'

curl -H 'Authorization: Bearer '$ACCESS_TOKEN localhost:3000/todo


```

## Resource
