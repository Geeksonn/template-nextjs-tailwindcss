This is a NextJS application with pre-installed tailwindcss. 

It serves as a template for quickly creating new NextJS+Tailwindcss app. 

## Procedure to re-create this template

``npx create-next-app app-name
cd app-name
npm i -D tailwindcss postcss autoprefixer
npx tailwindcss init -p``

Then, edit the `tailwind.config.js` to have:

``/** @type {import('tailwindcss').Config} */
module.exports = {
    content: ['./pages/**/*.{js,ts,jsx,tsx}', './components/**/*.{js,ts,jsx,tsx}'],
    theme: {
        extend: {},
    },
    plugins: [],
};``

Finally, in the `styles/global.css`, add these at the beginning of the file: 

``@tailwind base;
@tailwind components;
@tailwind utilities;``