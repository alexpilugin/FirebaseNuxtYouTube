# firebase-nuxt

Based on Youtube Tutorial: [https://www.youtube.com/watch?v=TjQsOy-8Wqo](https://www.youtube.com/watch?v=TjQsOy-8Wqo)    


> My pet Nuxt.js project for learning different approaches for ssr (server-side rendering) on Firebase

## Build Setup

``` bash
# install dependencies
$ npm i

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

## At first glance

SPA - single-page applications    
Static Site - pre-rendered or static-generated site
SSR - server-side-rendered application

I inserted small amendments in the nuxt.config.js file: ```ssr: true,``` instead of ```mode: "universal"```. But based on information in README file it looks like the project will be generated as a static site and will be deployed on Firebase Hosting...

## Project settings

Open Google Firebase Console and create a new firebase project:     
[https://console.firebase.google.com/u/0/](https://console.firebase.google.com/u/0/)    
Add a new web application to the project    
Copy firebaseConfig into ```/plugins/firebase.js``` file:    
```
const firebaseConfig = {
  apiKey: "",
  authDomain: "",
  projectId: "",
  storageBucket: "",
  messagingSenderId: "",
  appId: "",
  measurementId: ""
};
```

Link the current Nuxt project with a Firebase:
```
firebase logout
firebase login
firebase init
# select an existing project
```
