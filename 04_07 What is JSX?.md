# What is JSX?

### THIS IS A EXAMPLE OF JSX CODE

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

### SAME CODE, IF WE CONVERT THE JSX CODE INTO JAVASCRIPT CODE WITH BABEL
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
উদাহরন সরূপ একটা ইলিমেন্ট এর জন্য JSX এর পিছনে থাকা Object এর শেফ দেখানো হল।
```JS
const element = {
  type: 'div',
  props: {
    className: 'test',
    title: 'Test Me'
  },
  children: ['p', 'h1', 'img'] | 'Test' | null
}
```
