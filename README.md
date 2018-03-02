# myreactredux-starter-naveen
A quick starter for react on redux. 
Made it very simple by writing through each line of code
to undestand react on redux better.

*Hot Reload disabled*
as it would be too much of clutter in one go. 
It can be enabled in webpack.config.js

Instead of server.js , webpack dev server can be used for deploying app. 
Mainly depends on the convenience of the developer.

An ideal flow for understanding architecture of any such app would be 
1) Go through package.json and check for scripts
2) Inspect webpack.config.js and skim through all loaders.
3) Find the entry point in webpack.config.js and find out what are all the dependencies exist.
4) Check for presets if babel is used in .babelrc file.

A Typical React Redux Flow.

a) Declare pure functions aka reducers which would take an action and return a new state.
   (purity and immutability the key crux of REDUX). src/reducers/
b) Combine all reducers. src/reducers/index.js
c) Create a store using this combined reducer. src/index.js
d) Create all necessary components. src/components
e) Create a container that would link these components with the store created in step c
d) Have a main component where all the containers would be included. src/components/JSX
e) Include this main component in our entry file. src/index.js
f) Attach store to our main component by enclosing it inside Provider tag. src/index.js
g) Mount the component(class or function) returned in the above step to appropriate DOM element.

Happy Coding. :)
Do suggest any changes.
I would still recommend people to have handson experience than to completely rely on 
any starter/boiler project.





