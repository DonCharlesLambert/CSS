# React
## Introduction
[React](https://reactjs.org/), created by Facebook, is an open-source JavaScript library for building user interfaces. It is used to create components, handle state and props, utilize event listeners and certain life cycle methods to update data as it changes.

React combines HTML with JavaScript functionality to create its own markup language, JSX. This section will introduce you to all of these concepts and how to implement them for use with your own projects.

```
npx create-react-app my-app
cd my-app
npm start
```

## Introduction to JSX 
	const  JSX = <div></div>;
JSX is a syntactic extension of JavaScript, you can write JavaScript directly within JSX. To do this, you simply include the code you want to be treated as JavaScript within curly braces: 

	{ 'this is treated as JavaScript code' }
	
  
JSX is not valid JavaScript, JSX code must be compiled into JavaScript. The transpiler Babel is a popular tool for this process.  

Notes:
* Nested JSX must return a single element.
```JSX
const  JSX =
<div>
	{/* Renders Snake Stuff */}
	<h1> 🐍  Compiler </h1>
	<p> Snake, Snake </p>
	<ul>
		<li> Python </li>
		<li> Java </li>
		<li> Javascript </li>
	</ul>
</div>
```

*  These elements can be rendered using ReactDOM.render()
```JSX
const mainDiv = document.getElementById('main')
ReactDOM.render(JSX, mainDiv)
```
* Differences between HTML are className is used to give classes rather than class (class is reserved in JS, durr)
* Functions such as ```onclick()``` in HTML become camelCase (i.e ```onClick()``` in JSX

```JSX
const JSX = (
	<div className="myDiv" onClick={()=>console.log("yes"}>
		<h1>Add  a  class  to  this  div</h1>
	</div>
);
```
* Every tag must close, all tags can self-close

## Stateless Functional Components

```JSX
const sfc = function() {
	return(
		<div>
			Why  even  learn  HTML  when  JSX  exists
		</div>
	);
}
```
Can be nested into another component using
```JSX
<sfc/>
```

## React Components
```JSX
class TypesOfFood extends React.Component {
	constructor(props){
		super(props);
	}

	render(){
		return(
			<div>
				<h1>Types  of  Food:</h1>
				<Fruits/>
				<Vegetables/>
			</div>
		);
	}
};
```

Can be nested into another component using
```JSX
<TypesOfFood/>
```
Can be rendered using
```JSX
ReactDOM.render(<TypesOfFood/>, mainDiv)
```

## Component Notes
* Passing Props
```JSX
<Profile name="Bob Duncan"/>
```
* Setting default props
```JSX
Profile.defaultProps = {name: "John Doe"}
```
* Setting props types
```JSX
import PropTypes from 'prop-types';
MyComponent.propTypes = { handleClick: PropTypes.func.isRequired }
```

* Declaring inital state for React Components
```JSX
constructor(props){
	super(props);
		this.state = {
			name: "Bob"
		}
}
```
* Setting state
```JSX
	this.setState({
	  username: 'bobduncan125'
	});
```
* Setting state using previous state
```jsx
this.setState((state, props) => ({
  counter: state.counter + props.increment
}));
```
Remember that `setState()` is asynchronous, can use callback methods
Note that you have to wrap the object literal in parentheses, otherwise JavaScript thinks it's a block of code.

* Binding `this` in a function
```JSX
this.handleClick = this.handleClick.bind(this)
```
Can also just use arrow syntax