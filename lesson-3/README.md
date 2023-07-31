# tutoril video from min 20
https://www.youtube.com/watch?v=lCxcTsOHrjo

Starts at:
1:08 hr

* Check Steps in <lesson-1> & <lesson-2>

# Steps:
1. package.json. Change the name of the app
  "name": "lesson-3",

2. Run tailwind so it will "watch" the changes

3. 1:12 - 1:26
Work on the testimonial section. Use of pseudoclasses. Shit load of codes. This is a pain in the ass. 

4. 1:26- 1:32
Contact section. Form and button styling. Shit load of class again!

5. 1:32 - 1:39
Footer section. 
* Explanation of how to make invisible an element in cellpohone viewpoint and visible when it is ipad of bigger
<nav class="hidden md:flex flex-col
* How to create a media query responsive
<section class="max-w-4xl mx-auto p-4 flex flex-col sm:flex-row sm:justify-between">
- max-w-4xl. Define wider extstion of the elements in this section
- mx-auto. equal margin to the left and the right.
- flex flex-col sm:flex-row sm:justify-between. The elements are arranged as columns in cellphone viewpoint <sm> and once it hits the break point bigger than <sm> then the align in rows with <justify-between> which distribute the elements in the space. It looks good this way, it's very common to use.

6. 1.39 -1:45 Explanation of how to make visible only one section in the view port. This issue is solved eaier with framewors. I will have it here just in case in the future I need to have such a thing with a plain app 

* Changes in <input.css>, <tailwind.config.js> and <index.html>
input.css:
 @layer utilities {
     .section-min-height {
         min-height: calc(100vh - 68px)
     }
 }

tailwind.config.js:
      screens: {
        'widescreen': { 'raw': '(min-aspect-ratio: 3/2)' },
        'tallscreen': { 'raw': '(min-aspect-ratio: 1/2)' },
      }

index.html:
widescreen:section-min-height tallscreen:screen:section-min-height
* This is applied to each section so it will show only the section in the view point. Again this is not an issue with frameworks.