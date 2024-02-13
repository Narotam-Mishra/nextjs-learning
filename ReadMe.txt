
# Official website of NextJs - https://nextjs.org/

# Github link - https://github.com/mschwarzmueller/nextjs-complete-guide-course-resources/tree/main

# Basics of Next JS

# Next JS is full stack React framework, builds on top on Reactjs.

# NextJS vastly simplifies the process of building fullstack applications with React.

# Note - A standard React app is manipulated on the client in browser. As we know React js by default is a client side JS library which means it runs in the browser and it edits and manipulates the page in the browser.

# The main problem React App is that search engine crawlers don't see the actual page content if they visit the page for the first time and that's the difference with Nextjs. In Nextjs, we used to get all content not just visually on the screen but in the actual source code, because in Nextjs we no longer have a client-side application. Instead we have a full stack application.

# Note - With Nextjs we no longer have a client-side application, instead we have full stack application. With Nextjs projects, we have code that runs on the client and we have lots of code that runs on the server. Nextjs is simply both. It's not just client side-side, not just backend, it's both and Nextjs seamlessly blends client and server-side so that we can use React to build amazing full stack applications

# Page Router & App Router :- Both are simply two different ways of building NextJS apps.

# Page Router - It has been around for many years and is very stable. It is used in many existing NextJs projects that allow us to build feature-rich fullstack apps with React.

# App Router - It is intoduced in NextJS 13. Marked as stable but still realatively new and partially buggy. It supports modern Next & React features (fullstack React apps). The future of NextJS.

# Section-3 Nextjs Essentials (App Router)

# page.js and layout.js in app folder are reserved file names.

# 'page.js' file simply tells Nextjs that it should render a page.

# The special thing about 'page.js' is that it is so called server component,

# A type of component that's not really easily built with just React, but that is embraced and supported by NextJS.

# 'page.js' is a regular React component but treated in a special way by NextJS. It is treated as a server component and executed on the server and then it returned JSX code that sent over the wire to the browser to be rendered as HTML.

# `layout` is also reserved name for NextJS app.

# 'page.js' file defines the content of a page where as 'layout.js' defines the shell around one or more. Layout as the name suggests into which a page will be rendered.

# Note - Every Nextjs project needs at least one root 'layout.js' file.

# Note - 'metadata' defined in 'layout.js' file is also a reserved name

# `layout.js` and `page.js` work together. Layout is the wrapper where as page is the actual content.

# 'global.css' file is available globally for all files & folder inside root `app` folder.

# Note - If we add an image called 'icon' in app folder then it will be used as a favicon by NextJS as we can seen in 'layout.js' file we did not set up anything regarding a favicon.

# Note - The 'app' folder of NextJS is very important where we defines the routes by adding folders and we have some reserved file names like 'page.js' , `layout.js` & `icon.png` etc which then simply unlock different features.

# we can also create Regular React components which are not treated as pages.

# Usually we keep our components folder otside of the app folder, so that the app folder is just used for routing and routing related tasks.

# New feature used in NextJS projects where we can use '@' symbol in the import paths to refer to the root project. So, the root project outside of the app folder i.e a `jsconfig.json` file that configure this alias and that is simply convenience feature that can simplify our import paths.

# Reserved Filenames

# As you already learned, there are some reserved filenames when working with NextJS.

# Important: These filenames are only reserved when creating them inside of the app/ folder (or any subfolder). Outside of the app/ folder, these filenames are not treated in any special way.

# Here's a list of reserved filenames in NextJS - you'll, of course, learn about the important ones throughout this section:

# page.js => Create a new page (e.g., app/about/page.js creates a <your-domain>/about page)

# layout.js => Create a new layout that wraps sibling and nested pages

# not-found.js => Fallback page for "Not Found" errors (thrown by sibling or nested pages or layouts)

# error.js => Fallback page for other errors (thrown by sibling pages or nested pages or layouts)

# loading.js => Fallback page which is shown whilst sibling or nested pages (or layouts) are fetching data

# route.js => Allows you to create an API route (i.e., a page which does NOT return JSX code but instead data, e.g., in the JSON format)

# You also find a list with all supported filenames & detailed explanations in the official docs: https://nextjs.org/docs/app/api-reference/file-conventions

# Dynamic Route setup in NextJS

# Dynamic route - A route which we only define once but which is then capable of rendering different pages for different items. In NextJS, we can create such a dynamic route by adding a nested folder where we use square brackets. It is a special syntax supported by NextJS where we put any placeholder, any identifier of your choice between those square brackets, for example 'slug', and this placeholder become important later then again we need a `page.js` file to render some content.

# The square bracket ([]) thing there in folder name simply tells NextJS that we want to have some path segment after blog in this case but that we don't know the exact value of the segment yet then the placeholder, the identifier ([slug]) that will give access to the concrete value that we do get when that route is loaded. It is because NextJS- actually passes a props object to all those page components and all those page components get one special prop which we can pull out with help of destructuring and that is 'params' prop which is again set by NextJS. We don't have to pass it manually because we are not rendering these components manually.

# Inside the 'params' prop there is an object where every placeholder we had in such a dynamic route here will be a key and the value stored under that key wil be concrete value encoded in the URL. Example : /post-1

# 
