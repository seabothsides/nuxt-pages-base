---
title: more stuff and features
description: How to extend a sigle page app to more
---

## Layouts

the default layout holds the app nav bar

this nav bar iterates over arrays, one that holds the route names and the other holding names you would like to be displayed in the button

this can be moved to a component, or better yet the iretable list could be in a nuxt content file - like one called `options.md`

## Pages

The pages themselves simply call the content page that corresponds to the route. This can be altered to use a `_slug.vue` but can be a little messy in terms of having html tags for each data set that could come

The pages are were styles and layouts are implemented

## Content

The content file holds all data and content. Making it super easy to edit and update

You don't have to use the body either, you could simply refer to each content page like a JSON object
