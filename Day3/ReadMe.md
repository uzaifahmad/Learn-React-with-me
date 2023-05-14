# React Learning Journey - Day 3

## State and Events in React

In Day 3 of our React learning journey, we will explore state and events in React. State allows us to manage data within a component, while events enable interactivity and user-driven actions.

### Managing State

In React, state is an object that represents the data specific to a component. We can update and access the state using the `useState` hook.

#### Adding State to a Component

Let's add state to our `Greeting` component from Day 2, and display a dynamic greeting message based on user input.

1. Open the `src/Greeting.js` file.
2. Replace the existing code with the following code:

```jsx
   import React, { useState } from 'react';

   function Greeting() {
     const [name, setName] = useState('');

     const handleChange = (event) => {
       setName(event.target.value);
     };

     return (
       <div>
         <h1>Hello, {name || 'React'}!</h1>
         <input type="text" value={name} onChange={handleChange} />
       </div>
     );
   }

   export default Greeting;
```
### Handling Events
React provides event handling capabilities to handle user interactions, such as button clicks or form submissions.

Adding an Event Handler
Let's add an event handler to our `Greeting` component to display an alert when a button is clicked.

1. Open the src/Greeting.js file.
2. Add the following code inside the `Greeting` component, below the `<input>` element:
```jsx
const handleClick = () => {
  alert(`Hello, ${name || 'React'}!`);
};
```
3. Update the JSX code to include a button and attach the event handler:
```jsx
return (
  <div>
    <h1>Hello, {name || 'React'}!</h1>
    <input type="text" value={name} onChange={handleChange} />
    <button onClick={handleClick}>Click Me</button>
  </div>
);
```
### Commit: Add State and Event Handling to Component
Commit your code to mark the addition of state and event handling to the `Greeting` component. Use Git version control to create a new commit with an appropriate message.

Congratulations! You have learned how to manage state and handle events in React. Stay tuned for Day 4, where we will explore component lifecycle and hooks.


