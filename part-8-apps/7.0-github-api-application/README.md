# 7.0 - Github Api Application

Much respect must be sent to Samer Buna for this awesome starter app using the Github Api. It's a great starter app, and we'll use it to get started.

Here's your challenge: 1. We're going to give you the code for the files with minimal explanation. 2. You'll need to put the code into proper files to make it work. 3. Make the folders, make the files, make the routes, etc. 4. You have the jigsaw pieces, put them in place. 5. The app is also in a pretty sad state. Make it look nicer than it is.

## Overview

This application is pulling it's data from the GitHub API. We will be able to see a few details about a user after searching their username. The app will also show how to add the users to a list and we can store that on screen.

We need to first create a route for the incoming files, first we import it:

```javascript
import GithubCardApp from '../apps/github-api-app/GithubApp';
import GithubCardAppWithSearch from '../apps/github-api-app/GithubCardAppWithSearch';
```

Then we can add on to the route array:

```javascript
    {
      path: '/githubsimpleapi',
      exact: true,
      main: () => <div><GithubCardApp /> <br /> <GithubCardAppWithSearch /> </div>
    },
```

Now this will throw an error initially, so you can comment out this code until you are finished with building out the modules.

