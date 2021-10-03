## Tip Tuesday

#### Destructuring Props in React

- Destructuring was introduced in ES6
- It allows us to extract multiple pieces of data from an array or object and assign them to their own variables.
- How do we ensure a similar setup for Android devices?
- Let’s take a code example where we’re passing in a name and an emoji to a component that will display it-

#### import React from "react"
#### const EmojifyComponent = (props) => {
####  const { name, emoji } = props
#### return (
####   <h1>
####    {emoji} {name} {emoji} 
####   </h1>
####  )
#### }
#### export default EmojifyComponent


- Here’s the same exact React function component without destructuring:
#### import React from "react"
#### const EmojifyComponent = (props) => {
####  return (
####    <h1>
####      {props.emoji} {props.name} {props.emoji}
####    </h1>
####  )
#### }
#### export default EmojifyComponent 
 
```

```
- It’s not a big difference in such a small component, but in a React component with dozens of props, destructuring can be a big deal for readability.

-There's one more way of destructuring where we don't have to use the word props at all. The code for the same can be found in the index.js file.

#### Property

- Props Destructuring

#### Resources( To Learn More about SafeAreaView)

- https://reactnative.dev/docs/props
- https://medium.com/@lcriswell/destructuring-props-in-react-b1c295005ce0