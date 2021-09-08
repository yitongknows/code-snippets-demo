## Interacting with React state with Hooks
To declare a new variable in the state, we can use the `useState` hook. The `useState` hook initializes a variable; it also returns a function to update this state variable.

> Note: here we use the square brackets `[]`. Not the curly braces `{}`.
> We use curly braces to destructure objects, and square brackets to destructure arrays.
> For more detailed explaination, [see here](https://zellwk.com/blog/es6/#destructuring)
> 
```jsx
function App(){
const [currentState, setCurrentState] = useState("current state");

return(...);
}
```
