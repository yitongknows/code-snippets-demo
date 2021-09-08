## props is used to pass variables from one component to another component

In App.js, we have two variables `user` and `age`. We want to pass these variables to the `UserCard` component:
```jsx
function App(){
const user = "Bob";
const age = "10";

return(
  <UserCard user={user} age={age}/>
)}
```

In `UserCard.js`:
```jsx
const UserCard = (props) => {
    const { user, age } = props;

    return (
        <div className="user-card">
            <h1>{user} is {age} years old</h1>
        </div>
    );
};
```
