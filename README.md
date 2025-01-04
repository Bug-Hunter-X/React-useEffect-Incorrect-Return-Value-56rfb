# React useEffect Incorrect Return Value
This example demonstrates a common mistake in React's `useEffect` hook: returning a value that is not a cleanup function.  This can lead to memory leaks and unexpected behavior.

The `bug.js` file contains the problematic code.  The `bugSolution.js` file shows the corrected version.

## Problem
The `useEffect` hook in `bug.js` returns the number `1` instead of a cleanup function.  This is incorrect and can cause issues.

## Solution
The `bugSolution.js` file demonstrates the correct way to use the `useEffect` hook with a cleanup function.  The cleanup function ensures that any side effects, such as subscriptions or timers, are properly cleaned up when the component unmounts or when the dependencies change.