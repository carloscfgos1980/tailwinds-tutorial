## Class # 4. Nav Bar Animated 1:45 -2:33 hr
https://www.youtube.com/watch?v=lCxcTsOHrjo

# Goals:
- Add an animated hamburger manu (toggle nav bar)
- manu that shows up and also is animated


1. 

                <button id="hamburger-button" class="text-3xl md:hidden focus:outline-none">
- md:hidden. This button disappear when the viewpoint is ipadsize

<nav class="hidden md:block space-x-8 text-xl" 
- hidden md:block. The contrary of the button. The nav bar appears when the viewpoint is bigger than the ipad size


2. tailwind.config.js. Animation Explanation 2:00.
- It requires changes in <tailwind.config.js>, <index.html> and create a folder for javaScript <js>, inside the file <main.js>
2.1- Add the animation configuration. tailwind.config.js:
      keyframes: {
        'open-menu': {
          '0%': { transform: 'scaleY(0)' },
          '80%': { transform: 'scaleY(1.2)' },
          '100%': { transform: 'scaleY(1)' },
        },
      },
      animation: {
        'open-menu': 'open-menu 0.5s ease-in-out forwards',
      }

2.2 Add animation classes to the humgurger button index.html:
            class="absolute top-0 bg-black w-full text-5xl flex-col justify-content-center origin-top animate-open-menu hidden"
* We have to delete <flex> and add <origin-top animate-open-menu hidden>

2.3 Create the javaScrpt file in order to hide and make visible the button. main.js: Explanation 2:04
const initApp = () => {
    const hamburgerBtn = document.getElementById('hamburger-button')
    const mobileMenu = document.getElementById('mobile-menu')

    const toggleMenu = () => {
        mobileMenu.classList.toggle('hidden')
        mobileMenu.classList.toggle('flex')
        hamburgerBtn.classList.toggle('toggle-btn')
    }

    hamburgerBtn.addEventListener('click', toggleMenu)
    mobileMenu.addEventListener('click', toggleMenu)
}

document.addEventListener('DOMContentLoaded', initApp)

2.4 Add the javascript to the html. index.html:
    <script src="js/main.js" defer></script>

2.5 Tell tailwind to watch changes in the javascript files too. tailwind.config.js:
  content: ["./build/*.html", "./build/js/*.js"],

3. Second way. Animate the hamburger button. Explanation start 2:13 hr
@ This is a pain in the ass. i will never do such a thing... This guy build the whole animated hamburger button from scratch. I need to disable the CSS format for this projevt and then put it back again


THE END

# LESSON # 5 it is about deploying this app online which I am not interested to.