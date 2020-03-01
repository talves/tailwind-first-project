# tailwind-first-project

A simple website to demonstrate a responsive setup landing page without any custom css in using `tailwind`.
Tailwind is "A utility-first CSS framework for rapidly building custom designs." 

### Setup

```sh
yarn init -y
yarn add tailwindcss postcss-cli autoprefixer
npx tailwind init

```

Create postcss.config.js
```js
module.exports = {
  plugins: [require("tailwindcss"), require("autoprefixer")]
};

```

Script to run our base tailwind.css file

```js
  "scripts": {
    "build": "postcss css/tailwind.css -o public/build/tailwind.css"
  },
```