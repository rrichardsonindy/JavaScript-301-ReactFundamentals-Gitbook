# 5.0 - Movie Search Application

The next app we're going to build is a movie search app using [this](https://www.themoviedb.org/documentation/api) API.

## What We're Going to Build & Learn

* First, we'll build an input that allows users to search for movies in a database. We'll also display results based on what they type. 
* We're going to learn how to use `styled-components` inside each of our React files, to easily style things.
* The second part of the app we'll build is a section showing new movies at the box office. Here we'll learn more about utilizing APIs in react.

## Folder Structure

To start off our application, let's go ahead and make a folder for this application called `movie-search-app` inside of our `apps` folder. We'll also add 3 files to help you out.

```text
    └── src
        └── assets
        └── components
                └── apps
                    └── movie-search-app
                        └── Form.js
                        └── FormResults.js
                        └── MovieApp.js
```

## Routes

Next, we need to configure out links/routes , so first inside of `Sidebar.js` insert the following link:

```javascript
<li><Link to="/movie">Movie Search App</Link></li>
```

In `Sidebar.js` add the following route.

```javascript
<Route exact path="/movie"><MovieSearchApp /></Route>
```

You'll also need to set up the import for the `MovieSearchApp` component:

```javascript
import MovieSearchApp from '../apps/movie-search-app/MovieApp';
```

## MovieApp.js

Now that we've set up our routing so that our app can find our new Movie App, let's go ahead and add our parent component file. Inside of `movie-search-app` create your first file called `MovieApp.js`.

Let's go ahead and set up our parent component. Type the following code below into your `MovieApp`.

```javascript
import React, { Component } from 'react';
import { Form } from './Form';

export default class MovieApp extends Component {
    render() {
        return (
            <div className="main">
                <div className="mainDiv">
                    <Form />
                </div>
            </div>
        );
    }
}
```

Next, we'll start on our Form component!

[Movie Form Component](5.1-form-component.md)

