# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug: an infinite loop caused by the `useEffect` hook.  The `useEffect` hook, when used without a dependency array, runs after every render, triggering a continuous re-render cycle.  This example highlights the problem and provides a solution.

## Bug
The `bug.js` file contains the buggy component.  The `useEffect` hook, lacking a dependency array, runs on every render, causing the component to update repeatedly, resulting in an infinite loop.

## Solution
The `bugSolution.js` file demonstrates the corrected code.  By adding the `count` variable to the dependency array, `useEffect` only runs when the `count` value changes.