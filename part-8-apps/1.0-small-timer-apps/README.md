# 1.0 - Small Timer Apps

## What We're Going to Build & Learn

* A collection of time based apps
* This app will include a lot of use of lifecycle methods, as well as props and state practice.

## Getting Started

Before we start on our first timer app, we first need to add a folder for this app to our files. Underneath our apps folder, create a new folder called "timer-apps".

```text
    └── src
        └── assets
        └── components
                └── apps
                    └── timer-apps
```

Inside of our timer-apps folder, we're going to create our components for this timer application. The first component we will make will be the parent component for this app, like App.js is for our overall React application. Create a file called "TimePiecesApp.js" inside our timer-apps folder. Ensure, like always, that this is capitalized, as it is a react component.

```text
    └── src
        └── assets
        └── components
                └── apps
                    └── timer-apps
                        └── TimePiecesApp.js
```

In this application, we're going to learn more lifecycle methods, separating concerns in different components, and utilize some more ES6 functionality.

To get started we need to adjust our `_routes.js` and `Sidebar.js`, so that we have a way of navigating to our new mini-react app.

In your `_routes.js` file we need to add a route to our TimePiecesApp. Underneath the rest of your routes, you'll need to add one for the timer apps.

```javascript
    {
      path: '/timer',
      exact: true,
      main: () => <TimePiecesApp />
    },
```

Challenge: Go ahead set up the path by yourself. Hint: remember that the import path will be different now. We're no longer in the concepts directory.

In your `Sidebar.js`, you'll need to add a way to utilize this new route. Add the following to the file, underneath your other links.

```javascript
    <li><Link to="/timer">Timers</Link></li>
```

As our TimePiecesApp file is the parent component for our different little timer applications, we really only need our parent component in this instance to render the child components. Since we're not worried about state, we can go ahead and just make TimePiecesApp a functional component.

Go ahead and type the following code out in your TimePiecesApp.

```javascript
import React from 'react';
import TimerApp from './TimerApp';
import ClockApp from './ClockApp';
import StopWatchApp from './StopWatchApp'


const TimePiecesApp = () => {
    return (
        <div className="main">
            <div className="mainDiv">
                <TimerApp />
                <hr />
                <ClockApp />
                <hr />
                <StopWatchApp />
            </div>
        </div>
    )
}

export default TimePiecesApp;
```

When you try and run this, what do you think is going to happen? Go ahead and check out your app, and see if you were correct.

You should see an error like this:

```text
./src/components/apps/timer-apps/TimePiecesApp.js
Module not found: Can't resolve './ClockApp' in 'whereveryourappislocated/src/components/apps/timer-apps'
```

If you were correct, you would have guessed that it wouldn't run because it cannot find our TimerApp, ClockApp and StopwatchApp, since we haven't yet made them! In the next few chapters, we're going to go through each of these timer apps and create them.

## Simple Timer Setup

Next, we'll get started on setting up our first timer app!

[Simple Timer Setup](1.1-simple-timer.md)

