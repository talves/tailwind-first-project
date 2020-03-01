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