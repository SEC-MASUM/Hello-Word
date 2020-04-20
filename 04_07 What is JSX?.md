#What is JSX?

```JSX
import React, { Component } from 'react';

class App extends Component{
  render(){
    return (
      <div className='App'>
        <h1>What is JSX?</h1>
        <p>JSX is Awesome and it's Mean Javascript Extension</p>
      </div>
    );
  }
}
```

```JS
import React, { Component } from 'react';

class App extends Component{
  render(){
    return React.createElement('div', { classNmae: 'App'}, [
      React.createElement('h1', null, 'What is JSX?'),
      React.createElement(
        'p',
        null,
        'JSX is Awesome and it's Mean Javascript Extension'
      )
    ]);
  }
}
```
