## A JavaScript object can be used with a curly braces
```jsx
import React from 'react';

const GetUserName = (user) => {
  return user;
}

function App() {
  return (
    <div>
      <h1>Hello {GetUserName('Daisy')}</h1>
    </div>
  );
}

export default App;
```
