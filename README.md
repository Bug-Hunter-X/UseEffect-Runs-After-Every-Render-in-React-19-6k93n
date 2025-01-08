# React 19 useEffect Bug

This repository demonstrates a common issue in React 19 where the `useEffect` hook runs after every render, even when it shouldn't.  This can lead to performance problems and unexpected behavior.

## Bug Description
The `useEffect` hook in the provided `MyComponent` runs after every render, logging the current count to the console.  While this example is simple, in more complex applications, this behavior could significantly impact performance. 

## Solution
The solution involves using the optional dependency array in the `useEffect` hook to only run the effect when the `count` variable changes.

## How to Reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console logs—they will appear after every click.

