# Introduction

This sample project covers:

1. Setting up ImageKit Vue SDK in a NuxtJS app
2. Configuring ImageKit SDK in NuxtJS
3. Rendering images from ImageKit in NuxtJS
4. Resizing and cropping images in Nuxt applications
5. Converting Image Format with ImageKit in NuxtJS
6. Reduce image quality
7. Combining lazy loading with low-quality placeholders (LQIP)
8. Adding overlays to images

# How to run locally

## Install dependencies

```md
yarn install
OR
npm install
```

## Configuring ImageKit SDK in NuxtJS

In `plugins/imagekit-vue.js`, add the following block of code:

```js
import Vue from "vue";
import ImageKit from "imagekitio-vue";

Vue.use(ImageKit, {
  urlEndpoint: "<insert-your-url-endpoint>",
  publicKey: "<insert-your-public-key>"
});
```

Required parameters are `urlEndpoint` and `publicKey`

You can get the value of [URL-endpoint](https://imagekit.io/dashboard#url-endpoints) from your ImageKit dashboard.
API public key can be obtained from the [developer](https://imagekit.io/dashboard#developers) section in your ImageKit dashboard.

## Run the Nuxt app

```md
yarn dev
OR
npm run dev
```

Open the page at `http://localhost:3000`.## Run the Node.js server

# Useful links

- Vue quickstart guide - https://docs.imagekit.io/getting-started/quickstart-guides/vuejs
- Vue SDK and documentation - https://github.com/imagekit-developer/imagekit-vuejs

# Report a bug

If something doesn't work as expected, report a bug at support@imagekit.io.

### Credit:

This project was bootstrapped with [create-nuxt-app](https://nuxtjs.org/docs/2.x/get-started/installation#using-create-nuxt-app).
