
#Class Components

The idea of Components is essential in React. 

---

### Class Component Example

In the components folder, create a file called HelloWorld.js.

Add the following code to the file: 

```js
import React from 'react';
import {Component} from 'react';

export default class HelloWorld extends Component {
  render(){
    return(
      <div>Hello World</div>
    );
  }
}
```


### render(){}
In a class component, you must have the following items in every method:

```js 
render(){
  return(

  )
}
``` 

### Create instance of the component:



[9 - State](9-State.md)

