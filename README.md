# Unnecessary Re-renders in React useEffect Hook

This example demonstrates an inefficient use of the `useEffect` hook in React. The effect runs after every render, leading to unnecessary re-renders and console logs. The solution shows how to optimize the effect to only run when the `count` changes.

## Bug

The `useEffect` hook in the original `MyComponent` function runs after every render, causing performance issues and unnecessary console output. This can be problematic in larger applications.

## Solution

The improved `MyComponent` uses the `count` variable in the dependency array of the `useEffect` hook. Now, the effect only runs when the value of `count` changes, preventing unnecessary re-renders and improving performance.
