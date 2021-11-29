# Golang & Angular

Following [Golang & Angular Series - Part 1: Developing and Securing Golang APIs](https://auth0.com/blog/developing-golang-and-angular-apps-part-1-backend-api/)

[Developing a To-Do List Application with Angular](https://auth0.com/blog/developing-golang-and-angular-apps-part-2-angular-front-end/)

## Progress

Made it most of the way through part 2. Testing and debugging

## Notes

Getting git to ignore the files environment.ts and environment.prod.ts was more diffcult that I expected. The files were originally setup to be tracked. Once git starts tracking a file changing .gitingore for the file doesn't work. I needed to use the command `git update-index`.

``` shell
git update-index --skip-worktree ui/src/environments/environment.ts
git update-index --skip-worktree ui/src/environments/environment/prod.ts
```

## Starting the apps

for the API set the environment variables then run the app

```shell
export AUTH0_API_IDENTIFIER=<YOUR_AUTH0_API>
export AUTH0_DOMAIN=<YOUR_AUTH0_TENANT>.auth0.com

go run main.go
```

for the ui

```shell
ng serve
```

## Resource
