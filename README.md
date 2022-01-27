# site_refresh_project
! If error when run serve => check package.json =
```
REPLACE :
  "scripts": {
    "serve": "vue-cli-service serve",
    "build": "vue-cli-service build"
  },
 BY :
   "scripts": {
    "serve": "SET NODE_OPTIONS=--openssl-legacy-provider && vue-cli-service serve",
    "build": "SET NODE_OPTIONS=--openssl-legacy-provider && vue-cli-service build"
  },
```
## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
