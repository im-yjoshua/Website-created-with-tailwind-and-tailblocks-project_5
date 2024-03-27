## How to setup Tailwind CSS

Step 1:
Run the following Commands
```
npm install -D tailwindcss
npx tailwindcss init
```

Step 2:
Update the 'tailwind.config.js' file with:
```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
Step 3:
Create src/input.css to include:
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
Step 4:
Run the CLI tool to scan your template files for classes and build your CSS.
```
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```
**Step 5:** 
