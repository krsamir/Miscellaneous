# Passing Data Between React Components — Parent, Children, Sibling
***
### Three methods of Data Handling in React
1. From `Parent` to `Child` using `Props`
2. From `Child` to `Parent` using `Callbacks`
3. Between `Siblings` :
    * Combine above two methods
    * Using `Redux`
***
## From Parent to Child Using Props
![image1](https://github.com/krsamir/Miscellaneous/blob/master/Images/image%201.png)

Simply, use `this.props.dataFromParent` (just a variable used for sending props) to access the data sent from Parent to Child.

![image2](https://github.com/krsamir/Miscellaneous/blob/master/Images/image%202.png)

********************************
## From Child to Parent Using Callbacks
Let us suppose I need to send a message from Child1 to Parent — “Hello”. To do that, I need to follow a series of steps.

**Step 1**: Define a `callback function` that takes in a parameter which we consider having accessed `from the child in the Parent.js`<br>
**Step 2**: Also, `send the defined callback function as a props to the Child1.js`

![image3](https://github.com/krsamir/Miscellaneous/blob/master/Images/image%203.png)

**Step 3**: In `Child1.js` send the data using `this.props.callback`(dataToParent)

![image3](https://github.com/krsamir/Miscellaneous/blob/master/Images/image%204.png)
