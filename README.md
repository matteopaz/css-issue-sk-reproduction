# Reproduction
`npm install`
`npm run dev`

Now go notice how the global.css is being loaded with the red color style for h1s. This is being imported in __layout, so it should and does function always. This is a sanity check for global loading. 
Starting or reloading on the root page gives a red h1, and a black unstyled h2. When navigating to the subfolder, you recieve a red h1 and blue h2 as expected. When navigating back to index, the h2 has remained blue, loading the external stylesheet that is not being loaded on the current route.