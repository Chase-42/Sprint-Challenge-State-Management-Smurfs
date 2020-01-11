1. What problem does the context API help solve?

   Context API helps to solve the problem of prop drilling. It allows you to share data throughout an application without passing it manually.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

   "Actions": An object that carries data
   "Reducers": Pure functions that take the previous state and an action and return new state. '
   "Store": The state for the entire application as an Object.
   The single source of truth for the application where all immutable data is kept. Anytime you want to change data in the UI you have to dispatch an action to change the state via the reducer.

3. What is the difference between Application state and Component state? When would be a good time to use one over the other?

   Application state is for when you need state for the "global" application. It is useful for when you have many components that are in need of data.

   Component state is used for one component and is usually local to that single component. It is useful for when you only need state for a single component in your application and not for other components.

4. Describe `redux-thunk`, what does it allow us to do? How does it change our `action-creators`?

   "redux-thunk" is middleware that allows us to call action creators that return a function instead of an object. It delays the dispatch of the action to allow for asynchronous operations within the application. Useful for axios, etc.

5. What is your favorite state management system you've learned and this sprint? Please explain why!

   Redux is challenging and a little convoluted, but once you become familiar with it it is very organized, predictable and powerful. Very useful for passing state globally.
