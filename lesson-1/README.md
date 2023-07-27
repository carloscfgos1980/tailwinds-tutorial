## Lesson # 1

https://www.youtube.com/watch?v=lCxcTsOHrjo

npx tailwindcss init

* Til min 10 explanation from scratch

npx tailwindcss -i ./src/input.css -o ./build/css/style.css

npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch

# tailwindcss offitial website

https://tailwindcss.com/docs/installation

* Here we can find all the elements we need, just type it in the search bar

Some tailwindcss:
- grid place-content-center: It place the child component in the center
- bg-emerald-500. background color of thus div
- w-52 h-52. width and high of the div
- rounded-full. Give a round shape to the div

* Also global settings cab be place in  input.css and then and it as a class. Example
input.css
.radial-blue {
    background: radial-gradient(lightyellow, skyblue);
}
* This give a gradien background color center yellowish and border blueish
index.html:
<body class="min-h-screen grid place-content-center radial-blue">
