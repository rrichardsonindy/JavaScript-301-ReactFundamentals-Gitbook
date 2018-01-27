# State 


```js
import React from 'react';
import {Component} from 'react';


export default class IncrementButtonPartOne extends Component {
  constructor(props){
    super(props);
    this.state = {counter: 0};
  }
  render(){
    return(
      <button>{this.state.counter}</button>
    );
  }
}

```

### setState()

The setState() method allows us to change the state of something in our application.

```js
import React from 'react';
import {Component} from 'react';

export default class IncrementButtonPartTwo extends Component {
  constructor(props){
    super(props);
    this.state = {counter: 0}
  };

  incrementByOne = () => {
    this.setState({
      counter: this.state.counter + 1
    })
  };

  render(){
    return(
    
      <button onClick={this.incrementByOne}>
        {this.state.counter}
      </button>     
    );
  }
}
```
