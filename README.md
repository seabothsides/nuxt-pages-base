# nuxt-pages-base

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

## How to use this repo

This repo is made as an exmaple on how to use the nuxt content module to manage content for web pages.

unlike using the module for a collection of data, this is an example of using the content module to hold content that doesn't change all that often.

This way the conent is decoupled from the html and css code.

This decoupling means a CMS can be integrated a lot easier, especially netlify CMS

This example use the yaml and in the md file to hold conent that is generated into a JSON file for consumption on the front end.

The conent module also accepts .json file types which is more inline with CMS outputs like strapi
