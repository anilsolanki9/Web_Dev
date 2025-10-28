# Step 1

node install kro
check node and npm version

```bash
$node -v
$npm -v
```

# Step 2

Uske bad tumhara project folder vs code me open kar lo.
Then open terminal. Shortcut - `` ctrl + `  ``

Install tailwind version 3 hann old vala hi karna h, and uske sth postcss and autoprefixer and vite sab ek sath install kar lo

```bash
$npm install -D tailwindcss@3 postcss autoprefixer vite
```

Then

```bash
$npx tailwindcss init -p
```

# Step 3

Then kuch kam karne h woh suno......

- tailwind.config.js me jake content me `["*"]` add karna h. (below code jesa dikhna chahiye)

```js
module.exports = {
  content: ["*"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

- Then scripts add karni hai package.json me , (Below code jesa dikhna chahiye.)

```json
{
  "scripts": {
    "start": "vite"
  },
  "devDependencies": {
    "autoprefixer": "^10.4.21",
    "postcss": "^8.5.6",
    "tailwindcss": "^3.4.18",
    "vite": "^7.1.12"
  }
}
```

# Step 4

- create a main.css file and uske ander ye tin line add kar do

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

- Then css file ko html me link kar do.

```html
<link rel="stylesheet" href="main.css" />
```

- Then add any element and add any style to it

```html
<h1 class="bg-green-400">Hello brother</h1>
```

- add an extension in vs code --> [Tailwind css](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)

[![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-blue?logo=tailwindcss)](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)

- Then in terminal run

```bash
$npm run start
```

- Then usme vite link ayega uspe click karke output dekh skte ho. To exit press -

```bash
Ctrl + C
```
