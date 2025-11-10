Step 1. Terminal - `$npm init`

step 2. `$npm i vite`

step 3. `$npm install -D tailwindcss@3 postcss autoprefixer`

step 4. `$npx tailwindcss init`

step 5. create a file name - postcss.config.js and add this content to it

```js
module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  }
}
```
step 6. open `tailwind.config.js` and add "*" in its content 
```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["*"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
step 7. create any .cc file and add these three to it
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```
step 8. add start script to `package.json` file
```json
{
  "name": "tailwind_demo",
  "version": "1.0.0",
  "description": "",
  "license": "ISC",
  "author": "",
  "type": "commonjs",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "vite"
  },
  "dependencies": {
    "vite": "^7.1.12"
  },
  "devDependencies": {
    "autoprefixer": "^10.4.21",
    "postcss": "^8.5.6",
    "tailwindcss": "^3.4.18"
  }
}
```
step 9. link .css file to html

step 10. to start server - $npm start 
to exit server - $ctrl+c
