npm create vite@latest // this will add project name

cd to Project name

npm init -y

npm install -D tailwindcss@3 @tailwindcss/postcss autoprefixer

npx tailwindcss init -p

this is src/index.css

@tailwind base; @tailwind components; @tailwind utilities;

Latest way to install in 4.0

01.Install tailwindcss and @tailwindcss/cli via npm. a. create a folder when you want to install and CD to folder

npm install tailwindcss @tailwindcss/cli

b.creaate a SRC folder CD to SRC and create Input.css and index.html

inside input.css Add

@import "tailwindcss";

C. Start using Tailwind in your HTML

in SRC/index.html

<!doctype html>

Hello world!
D. Create the tailwind.config.js and add

module.exports = { content: [ "./index.html", "./src/**/*.{html,js}" // Include all relevant paths ], theme: { extend: {}, }, plugins: [], }

c. Start the Tailwind CLI build process

npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch