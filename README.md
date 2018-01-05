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

### Recommended Reading

1. [**React**](https://reactjs.org/docs/hello-world.html)

   It is not necessary to follow the official React tutorial if you have already completed the Codecademy courses for React. Make sure you understand the following items in the [**ADVANCED GUIDES**](https://reactjs.org/docs/jsx-in-depth.html) section:

   - [JSX In Depth](https://reactjs.org/docs/jsx-in-depth.html)
   - [Refs and the DOM](https://reactjs.org/docs/refs-and-the-dom.html)
   - [Reconciliation](https://reactjs.org/docs/reconciliation.html)
   - [Fragments](https://reactjs.org/docs/fragments.html)
   - [Error Boundaries](https://reactjs.org/docs/error-boundaries.html)

2. [**React-Router**](https://reacttraining.com/react-router/web)

   Traditionally, changes in the URL would be associated with visiting a new HTML page requested from the server. In single-page applications, rendering of content and communication with the server is done without visiting entirely new pages. Since new pages are not visted, the URL will not change. This is a problem because URLs are very useful for allowing users to use their built-in browser navigation buttons and use links to specific content.
   
   Many modern Javascript frameworks include URL routing functionality. This allows changes in the application state or appearance to be associated with a change in the URL. React does not include routing. Instead a separate library called [**React-Router**](https://reacttraining.com/react-router/web) used.

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
       - [Reducing Boilerplate](https://redux.js.org/docs/recipes/ReducingBoilerplate.html) \(ignore async action creators\)
       - [Writing Tests](https://redux.js.org/docs/recipes/WritingTests.html) \(ignore async action creators\)
       - [Structuring Reducers](https://redux.js.org/docs/recipes/StructuringReducers.html)

4. [**Redux-Saga**](https://redux-saga.js.org/)

   Redux is not well-suited to handling data asynchronously (eg. AJAX) by itself. There is Redux middleware available for dealing with this problem. We use Redux-Saga. Redux-Saga uses ES6 generators (read about them [here](https://goshakkk.name/javascript-generators-understanding-sample-use-cases/). Relevant sections of the docs are:

   - [Introduction](https://redux-saga.js.org/docs/introduction/)
       - [Beginner Tutorial](https://redux-saga.js.org/docs/introduction/BeginnerTutorial.html)
   - [Basic Concepts](https://redux-saga.js.org/docs/basics/)
   - [Advanced Concepts](https://redux-saga.js.org/docs/advanced/)
       [Running tasks in parallel](https://redux-saga.js.org/docs/advanced/RunningTasksInParallel.html)

5. [**Webpack**](https://webpack.js.org/)

   Webpack is used to turn the client source files into single bundled Javascript, CSS, and HTML assets for download by the browser. Relevant sections of the docs are:

   - [Concepts](https://webpack.js.org/concepts/)
   - [Loaders](https://webpack.js.org/concepts/loaders/)
   - [Plugins](https://webpack.js.org/concepts/plugins/)
   - [Configuration](https://webpack.js.org/concepts/configuration/)

6. [**Yarn**](https://yarnpkg.com)

   Yarn is used for Javascript package management. It helps to download and manage dependencies such as ``react``.

   - [Installation](https://yarnpkg.com/en/docs/install)
   - [Usage](https://yarnpkg.com/en/docs/usage)

## Javascript Style Guide

### 1. References

- Use ``const`` whenever possible. Use ``let`` otherwise.
- Don't use ``var``.

### 2. Objects

- Use literal syntax for object creation  .
  ```javascript
  // use
  const item = {};

  // not
  const item = new Object();
  ```

- Use property shorthand.
  ```javascript
  const value = "foobar";
  
  // use
  const item = {
      value
  };

  // not
  const item = {
      value: value
  };
  ```

- Group shorthand properties at beginning of object declaration.
  ```javascript
  const index = 0;
  const value = 2;
  const itemLabel = "a number";

  const item = {
      index
      value,
      label: itemLabel
  }
  ```

- Only quote properties when necessary.
  ```javascript
  const item = {
      "item-values": [0, 1, 2],
      label: "foobar"
  };
  ```

### 3. JSX

- use the spread operator when possible
  ```javascript
  const element = <Item {...props} />;
  ```
- leave a space at the end of one-line element definitions
  ```javascript
  const element = <SampleItem name="Test" />
  ```
- split long element definitions across multiple lines
  ```javascript
  const element = (
      <SampleList
          samples={sampleItems}
          show
      >
  );
  ```
- 
