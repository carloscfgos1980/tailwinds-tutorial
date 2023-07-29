# tutoril video from min 20
https://www.youtube.com/watch?v=lCxcTsOHrjo

* All the steps in lesson # 1 and then this:
# Steps:
1. 
npm init -y

2. tailwind.config.js:
  content: ["./build/*.html"],

3. package.json:
  "scripts": {
    "tailwind": "npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch"
  },

4. 
npm i -D prettier-plugin-tailwindcss

5. Create .gitignore and add node_modules so this folder will be ignored when the app is upload to git github

6. package.json
    "prettier": "npx prettier --write **/*.html"

7. npm run tailwind

8. index.html
8.1 type <!> then tap. This gives me the basic HTML format
8.2 Change the name <Acme Rockets>
8.3 Add css link:
    <link rel="stylesheet" href="css/style.css">
8.4 A bunch of styling
<body class="min-h-screen bg-slate-50 dark:bg-black dark:text-white">
- min-h-screen. Min high of the screen. Responsive
-  bg-slate-50. background of the page
-  dark:bg-black dark:text-white. Dark mode confifuration
- ticky top-0. Get hoold to the very top of the page
- z-10. ????
        <section class="max-w-4xl mx-auto p-4 flex justify-between items-center">
- max-w-4xl. Maximum window. The section no widther than 896 px (4xl)
- mx-auto. This makes equal margin both sides and make the section to the center.
- p-4. Padding all around the section
- flex justify-between. Flex bos for the childrem elements
-items-center. Childrem elements align to the center

* add h1 inside senction with the name of the app. Also get and emoij rocket. We can find emoijs in this website:
https://emojipedia.org/

button#mobile-open.button.text-3xl.sm:hidden.focus:outline-none
- button#mobile-open and <tap>. Creates a button with the ID <mobile-open>


The content of the butto is the hamburg ico. It is like this: &#9776
https://symbl.cc/en/

class="text-3xl sm:hidden focus:outline-none"
- sm: hidden. It hides the hamburg icon when it reaches <sm> break point. sm. it defines as min-width of 640 px.

                <nav class="hidden sm:block space-x-8 text-xl"></nav>
    
hidden sm:block. We dont see at first, and after that we set the media query to small <sm> with a block display
- hidden sm:block. This give the children of the nav element a margin left of  

aria-label="main. Set this nav as a the main in case there are other nav



        <section id="hero" class="flex flex-col-reverse justify-center sm:flex-row p-6 items-center gap-8mb-12">

- flex flex-col-reverse justify-center sm:flex-row. This place the second element to the right of the screen (large) and on the top of the screen (small)- view port


* Shitload of explanation. Check 1:107 for the scroll explanation