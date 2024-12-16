# React useEffect Hook Missing Cleanup Function

This repository demonstrates a common error in React: forgetting to include a cleanup function in the `useEffect` hook.  This can lead to memory leaks and unexpected behavior.

## Bug
The `bug.js` file contains a component with a `useEffect` hook that logs a message to the console when the component mounts. However, it lacks a return statement (the cleanup function) to handle cleanup actions when the component unmounts.  This means that the effects are not properly cleaned up.

## Solution
The `bugSolution.js` file demonstrates the corrected code. The `useEffect` hook now includes a return statement which ensures that cleanup happens when the component unmounts. This is essential for avoiding memory leaks and ensuring the component behaves as expected.