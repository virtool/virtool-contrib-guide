# virtool-contrib-guide

## Web Client Development

### Recommended Codecademy Courses

These online courses will help you understand the basics of the technologies used in the Virtool client.

1. [Learn HTML](https://www.codecademy.com/learn/learn-html)
2. [Learn CSS](https://www.codecademy.com/learn/learn-css)
3. [Make a Website](https://www.codecademy.com/learn/make-a-website)
4. [Intro to Javascript](https://www.codecademy.com/learn/introduction-to-javascript)
4. [Learn ReactJS: Part I](https://www.codecademy.com/learn/react-101)
5. [Learn ReactJS: Part II](https://www.codecademy.com/learn/react-102)

### Recommended Tutorials

1. [Git Tutorial](https://try.github.io)
2. []

### Recommended Reading

1. [**React**](https://reactjs.org/docs/hello-world.html)

   It is not necessary to follow the official React tutorial if you have already completed the Codecademy courses for React. The most important content for our purposes is in the [**ADVANCED GUIDES**](https://reactjs.org/docs/jsx-in-depth.html) section. Make sure you understand the following items found there:

   - JSX In Depth
   - Refs and the DOM
   - Reconciliation
   - Fragments
   - Error Boundaries

2. [**React-Router**](https://reacttraining.com/react-router/web)

   Traditionally, changes in the URL would be associated with visiting a new HTML page requested from the server. In single-page applications, rendering of content and communication with the server is done without visiting entirely new pages. Since new pages are not visted, the URL will not change. This is a problem because URLs are very useful for allowing users to use their built-in browser navigation buttons and use links to specific content. Many modern Javascript frameworks include URL routing functionality. This allows changes in the application state or appearance to be associated with a change in the URL. React does not include routing. Instead a separate library called [**React-Router**](https://reacttraining.com/react-router/web) used.

   Relevant documentation sections are:

   - [Examples](https://reacttraining.com/react-router/web/example/basic)
   - [API](https://reacttraining.com/react-router/web/api/BrowserRouter)
       - [``BrowserRouter``](https://reacttraining.com/react-router/web/api/BrowserRouter)
       - [``Link``](https://reacttraining.com/react-router/web/api/Link)
       - [``NavLink``](https://reacttraining.com/react-router/web/api/NavLink)
       - [``Redirect``](https://reacttraining.com/react-router/web/api/Redirect)
       - [``Route``](https://reacttraining.com/react-router/web/api/Route)
       - [``Switch``](https://reacttraining.com/react-router/web/api/Switch)
       - [``matchPath``](https://reacttraining.com/react-router/web/api/matchPath)
   
3. [**Redux**](https://redux.js.org/)

   Redux is used for state management. Many React components in the Virtool client take state from a central Redux data store. Relevant sections of the Redux docs are:

   - [Introduction](https://redux.js.org/docs/introduction/)
   - [Basics](https://redux.js.org/docs/basics/)
   - [Recipes](https://redux.js.org/docs/recipes/)
       - [Using Object Spread Operator](https://redux.js.org/docs/recipes/UsingObjectSpreadOperator.html)
       - [Reducing Boilerplate](https://redux.js.org/docs/recipes/ReducingBoilerplate.html) \(ignore async action creators \)
       - [Writing Tests](https://redux.js.org/docs/recipes/WritingTests.html) \(ignore async action creators \)
       - [Structuring Reducers](https://redux.js.org/docs/recipes/StructuringReducers.html)

4. [**Redux-Saga**](https://redux-saga.js.org/)

   Redux is not well-suited to handling data asynchronously (eg. AJAX) by itself. There is Redux middleware available for dealing with this problem.

5. [**Virtool Web API**](https://docs.virtool.ca/development/api/)

## Style

### Javascript and JSX

1. Modal Routing


