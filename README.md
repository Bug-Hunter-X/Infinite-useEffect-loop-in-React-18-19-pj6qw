# Infinite useEffect Loop in React 18/19

This repository demonstrates a common error in React applications involving the `useEffect` hook. The example showcases an infinite loop caused by an incorrectly defined dependency array, leading to performance degradation.

## Problem
The `useEffect` hook is designed to perform side effects after each render. However, if its dependency array is missing or incorrectly defined, it may run repeatedly and infinitely.

## Solution
The correct usage of the dependency array prevents the infinite loop by specifying that the effect should only run when the specific dependency changes.  This example correctly uses a dependency array containing 'count'. The effect only runs when the state variable 'count' updates.