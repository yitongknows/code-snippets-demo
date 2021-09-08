## Code snippet to show how to embed js in jsx
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
