# React 19 useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  Incorrectly specifying the dependency array in `useEffect` can lead to unexpected behavior, such as infinite loops.

## Bug Description

The `bug.js` file contains a component that uses `useEffect` to log a message to the console after every render.  However, the dependency array is missing, causing the effect to run repeatedly, creating an infinite loop.

## Solution

The `bugSolution.js` file shows the corrected code. By including `count` in the dependency array, the effect only runs when the `count` variable changes, thus resolving the infinite loop issue.  Always carefully define the dependencies for your `useEffect` calls to prevent unintended side effects.