# React 19 useEffect Hook Dependency Array
This repository demonstrates a common error in React 19 and its solution.  The example showcases the importance of correctly defining the dependency array within the `useEffect` hook to prevent unexpected behavior.

## Bug
The initial `bug.js` file demonstrates an incorrect usage of `useEffect` where the state variable isn't included in the dependency array.  This leads to the effect running on every render, potentially causing performance issues or infinite loops.

## Solution
The `bugSolution.js` file corrects the issue by adding `count` to the dependency array. This ensures the effect only runs when the value of `count` changes.

## How to run the example
1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.