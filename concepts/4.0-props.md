# Props

[demo](class-components) / [source](https://github.com/jpauloconnor/react-library/blob/master/src/components/Demo_01.js)

### Functional Components w/ props
Make a folder for all this.....


```js
import React from 'react';

const ReusableButton = function(props){
  return(
    <button>{props.label}</button>
  );
};

export default ReusableButton;
```


And here we have our App, where we can create many instances of the component, while passing any different props. Don't forget to import the component!

```js
class App extends Component {
  render() {
    return (
      <div className="App">
        <div className="App-header">
          <img src={logo} className="App-logo" alt="logo" />
          <h2>Welcome to React</h2>
        </div>
        <ReusableButton label="Press here" />
        <ReusableButton label="And press here" />
        <ReusableButton label="Another Button" />
        <ReusableButton label="You get the point" />
        <ReusableButton label="Hello" />
        <ReusableButton label="Another Button" />
      </div>
    );
  }
}
```

[8 - Class Components](8-Class-Components.md)

