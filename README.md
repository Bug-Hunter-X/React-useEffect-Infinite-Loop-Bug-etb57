# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by a missing dependency.  The `useEffect` hook is used to perform side effects, but if it's not properly declared with dependencies, it can lead to unexpected behavior.  The solution shows how to correctly specify dependencies to avoid this issue.

## Bug

The `bug.js` file contains the buggy code.  The `useEffect` hook is missing a dependency which creates an infinite loop.

## Solution

The `bugSolution.js` file shows the corrected code, where the `count` variable is added to the dependency array. This ensures the effect only runs when the `count` value changes.