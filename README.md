# Native Modular Components | proof of concept

This repo is for demonstrating the use case of using components-like structures to split the logic into isolated pieces

It can be seen online at: https://native-js-modular-components-demo-xzhfwtdjqh.now.sh/


This demo demonstrates:

- The use of classes to create components-like structures
- The use of a separate template files per component
- The use of a separate styles.css per component
- How [we can use ES6 modules in some browser](https://caniuse.com/#feat=es6-module)s 
- How we can somehow mount components into specific parts of our DOM
- A very basic implemenation of a Publish/Subscribe pattern that serves to communicate componentsnow

```
.
├── css
│   └── styles.css
├── index.html
└── js
    ├── app.js
    ├── components
    │   ├── App
    │   │   ├── index.js
    │   │   └── template.js
    │   ├── ListItem
    │   │   ├── index.js
    │   │   ├── styles.css
    │   │   └── template.js
    │   ├── ListResults
    │   │   ├── index.js
    │   │   ├── styles.css
    │   │   └── template.js
    │   └── Search
    │       ├── index.js
    │       └── template.js
    ├── config.js
    ├── libs
    │   └── EventEmitter.js
    └── services
        └── serviceApiMarvel.js
```


## Local Installation 

Clone the repo and add a `js/config.js` w/ your PUBLIC_KEY

```
export const PUBLIC_KEY = "b782c35caf4fb24ac96d9f4c832e3120"
```

Launch a local server and add your local url (usually `localhost`) to your authorized referrers in your Marvel Developer Account
