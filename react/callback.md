## Use Callback Handlers to Communicate Up

In section Props, we disscuss that we can only use props to pass data down the component tree, but cannot pass it upwards. 
However, we can bypass this limitation by using **callback handlers**.

In the example below, we first pass down the event handler `handleClick` (by reference) down to App's child component - `MyButton`. When the click event
is called in `MyButton`, the `handleClick` event is actually invoked at the `App` component level. This is called callback.

In App.js, we have:
```jsx
const App = () => {
const friends = [
    {
        name: "Bob",
        age: "21",
    },
    {
        name: "Anna",
        age: "23",
    },
];

const handleClick = event => {
  console.log(Json.Stringify(friends));
};

return(
<MyButton onClick={handleClick}/>
)
}
```
Then, in a custom component `MyButton`, we have:
```jsx
export const MyButton = (props) => {
  return(
    <Button onClick={props.handleClick}/>
  )
}
```
