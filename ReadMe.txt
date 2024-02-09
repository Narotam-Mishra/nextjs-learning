
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

# 'page.js' file defines the content of a page where as 'layout.js' defines the shell around one or more. Layout as the name suggests into which a page will be rendered.

# Note - Every Nextjs project needs at least one root 'layout.js' file.

# Note - 'metadata' defined in 'layout.js' file is also a reserved name

# `layout.js` and `page.js` work together. Layout is the wrapper where as page is the actual content.