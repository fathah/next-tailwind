# next-tailwind
_Common Setup for Next.js and Tailwind CSS_

## Create Next App
```sh
npx create-next-app .
```

## Setup Tailwind
#### 1. Install Tailwind
```sh
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
```
#### 2. Create configuration files
```sh
npx tailwindcss init -p
```
#### 3. Modify tailwind.config.js
```js
purge: ['./pages/**/*.{js,ts,jsx,tsx}', './components/**/*.{js,ts,jsx,tsx}'],
```
#### 4. Include Tailwind in CSS `styles/globals.css`
```css
@tailwind base;
@tailwind components;
@tailwind utilities;

```


## Setup AOS Animation
#### 1. Install AOS
```sh
npm i aos
```
#### 2. Configure AOS
Import and add in `_app.js`
```js
import AOS from 'aos';
import "aos/dist/aos.css";
import {useEffect} from 'react';

 useEffect(() => {
    AOS.init({
      easing: "ease-out-cubic",
      once: true,
      offset: 50,
    });
  }, []);
```


## Setup React Icons
#### 1. React Icons

```sh
npm i react-icons
```
#### 2. Find Icons

[`Search For Icons`](https://react-icons.github.io/react-icons)



