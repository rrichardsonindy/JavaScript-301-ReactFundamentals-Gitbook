# jsx

Use babeljs.io to show example from first functional component....

JSX gets compiled into vanilla js.

You can write it without, but not many people do that....

```js

import React from 'react';
import { Component } from 'react';
import Codepen from 'react-codepen';


export default class JSXRules extends Component {
	render(){
		return(
			<div className="main">
				<div className="mainDiv">
					<h1 className="section-title">JSX</h1> 

					<dl>
						<dt>This looks familiar...</dt>
					    <dd>JSX looks like HTML, but it's not. It's actually closer to JavaScript.</dd>
					    <dt>"React elements"</dt>
					    <dd>These are used to construct and update the DOM, what you see on the screen.</dd>
					    <dt>Components can't return multiple React elements</dt>
					    <dd>To bypass you must wrap everything in a component in one element( div, h1, p, etc.)</dd>
					    
					</dl>

					<p>This looks like some crazy hybrid of JavaScript and HTML! Really it's just a different
					syntax for JavaScript. You can embed JavaScript expressions in JSX by wrapping them in curly braces .</p>
					<p>The most important thing to notice below is the way JSX treats classes. Since it is like JavaScript, React DOM uses 
					camelCase in naming. So instead of class, you use className. This also happens because class is already a keyword in React
					(remember Class Components?).</p>
				</div>
			</div>
		);
	}
}

```

[7 - props](7-props.md)
