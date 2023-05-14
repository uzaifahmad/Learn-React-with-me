# React Learning Journey - Day 2

## React Basics

In Day 2 of our React learning journey, we will cover the basics of React. We will understand React components and JSX syntax, create a simple functional component, and render it.

### React Components

React is built around components, which are reusable and independent pieces of UI. Components can be either functional or class-based.

#### JSX Syntax

JSX (JavaScript XML) is an extension to JavaScript that allows us to write HTML-like code within JavaScript. It is a syntax extension provided by React for creating React elements.

### Create a Simple Component

Let's create a simple functional component that displays a greeting message.

1. Create a new file in the `src` directory of your React project, named `Greeting.js`.
2. Add the following code to the `Greeting.js` file:

```jsx
import React from 'react';

function Greeting() {
  return <h1>Hello, React!</h1>;
}

export default Greeting;
```
### Render the Component
Now, let's render the Greeting component in the main App component.

1. Open the src/App.js file.
2.Replace the existing code with the following code:
```jsx
import React from 'react';
import Greeting from './Greeting';

function App() {
  return (
    <div>
      <Greeting />
    </div>
  );
}

export default App;
```
Commit: Create a Basic Component and Render It
Commit your code to mark the creation of a basic component and rendering it in the main `App` component. Use Git version control to create a new commit with an appropriate message.

Congratulations! You have learned the basics of React and created your first component. Stay tuned for Day 3, where we will explore state and events in React.
