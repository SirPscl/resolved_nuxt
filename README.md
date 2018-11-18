# resolved-nuxt

## Error redirect

Add to `.htaccess`:

```
ErrorDocument 404 /index.html
```

## Serve Static locally

``` bash
npm install -v serve
serve ./dist
```

## Build Setup

``` bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# serve with hot reload at <IP>:3000
$ HOST=0.0.0.0 npm run dev

# build for production and launch server
$ npm run build
$ npm start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, checkout [Nuxt.js docs](https://nuxtjs.org).

## Deployment
