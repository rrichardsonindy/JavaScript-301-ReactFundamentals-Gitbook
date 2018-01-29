#Components

Hopefully, you notice that we had separate files for header, footer, main, sidebar, etc. These are all known as components. React has two major types of components. Functional Components and Class Components.  Components are individual pieces of the UI that can be altered independent of one another. 

### Functional Components

* Functional components allow you to render information to the web page without having to use or change state.
* Functional components are known as presentation components.  
* Often used for simply rendering a small chunk of code to the dom.
* No 'this' keyword 
* Unlike class components, functional ones don't use 'this'. 
* Don't worry about changing state with these.
* These are dumb components for UI. 

### Class Components
* Have a mutable state in the application.
* Class components are considered the "React way" of writing components.  
* Extends React.Component. 
* You can write this as either "extends React.Component" or "extends Component" with Component being imported in from react at the top of your code.
* Must always have a render() method.

### Directory Setup
Let's set up a few files for the next Section. 

```
    └── src
        └── assets
        └── components
                └── concepts
                      └── ClassComponentDemo.js
                      └── FunctionalComponentDemo.js
                └── site
```
[5 - Functional Components](5-Functional-Components.md)
