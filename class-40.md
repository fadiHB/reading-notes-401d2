
## Pre-rendering.
By default, Next.js pre-renders every page. This means that Next.js generates HTML for each page in advance, instead of having it all done by client-side JavaScript. Pre-rendering can result in better performance and SEO.Each generated HTML is associated with minimal JavaScript code necessary for that page. When a page is loaded by the browser, its JavaScript code runs and makes the page fully interactive. (This process is called hydration.) (Links to an external site.)

## Check That Pre-rendering Is Happening (Links to an external site.)
You can check that pre-rendering is happening by taking the following steps: (Links to an external site.)
Disable JavaScript in your browser (here’s how in Chrome) and Try accessing this page (the final result of this tutorial). You should see that your app is rendered without JavaScript. That’s because Next.js has pre-rendered the app into static HTML, allowing you to see the app UI without running JavaScript.

## Development v.s. Production (Links to an external site.)
In development (npm run dev or yarn dev), getStaticPaths runs on every request.
In production, getStaticPaths runs at build time.
