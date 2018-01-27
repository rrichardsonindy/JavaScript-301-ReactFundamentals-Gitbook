# Getting Started with React
To get stared with React, we'll use Create React App. Starting out with Create React App allows us to get started locally with React without having to set up build configurations. Create React App works on macOS, Windows, and Linux. We just need to have Node.js installed.

If something doesn’t work, please contact your instructor immediately.

### Quick Start
Here are the steps that you will need to create your initial app. Note that the npx command is [correct](https://medium.com/@maybekatz/introducing-npx-an-npm-package-runner-55f7d4bd282b).


```sh
npx create-react-app react-fundamentals
cd react-fundamentals
npm start
```

Here's Facebook's starter screenshot for more help. Note that we are calling ours React Fundamentals:
<p align='center'>
<img src='https://cdn.rawgit.com/facebookincubator/create-react-app/27b42ac/screencast.svg' width='600' alt='npm start'>
</p>

### Open the App
Open [http://localhost:3000](http://localhost:3000) to view it in the browser. You should see the starter app:

### Adding a folder.
Before proceeding, please right click on teh src folder and add 3 folders: 'components', 'constants', and 'css'. Note: so that we can quickly get started with React, we can add SCSS files l

### App Overview
After creating the application in your terminal open up VS Code and open the react-fundamentals folder that contains the app. Take a look the files in the src folder and get an idea of where things are. For the most part, we'll be working in there. <br />

Do 5 minutes of orientation here. 

```
react-fundamentals
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── public
│   └── favicon.ico
│   └── index.html
│   └── manifest.json
└── src
    └── assets
    └── components
    └── constants
    └── styles
    └── App.css
    └── App.js
    └── App.test.js
    └── index.css
    └── index.js
    └── logo.svg
    └── registerServiceWorker.js
```

### Running the app

To run the app in VS Code, open your terminal by clicking Ctrl + `.

Then, run 
```sh
npm start.
```

You should get a message that the app is running on localhost:8080.



### Sass Setup
We'll get started on setting up SASS. 

[2 - Sass-Setup](2-Sass-Setup.md)








