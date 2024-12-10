# React Native Uninitialized State/Prop Access

This repository demonstrates a common error in React Native applications: accessing state variables or props before they've been initialized.  This typically leads to unexpected behavior, such as rendering undefined values or even application crashes.  The provided code showcases the problem and offers solutions.

## Problem
The `UninitializedState.js` file shows how accessing state variables (using `useState`) or props before they're assigned values can result in errors.  This often occurs within a component's render method or during asynchronous operations.

## Solution
The `UninitializedStateSolution.js` file illustrates how to address this issue.  Key solutions include:

* **Initializing state variables with default values:** Provide a default value to `useState` to prevent undefined values. 
* **Conditional rendering:** Check for undefined values before attempting to render them using short-circuiting logic or optional chaining.
* **Asynchronous handling:** Ensure props are properly accessed after the component has mounted by using lifecycle methods (`componentDidMount` or `useEffect`)

This repository serves as a learning resource to understand and avoid this common React Native pitfall.