# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook causing an infinite loop.  The issue arises from an improperly defined dependency array within the `useEffect` function.

## Bug Description

The `useEffect` hook is used to perform side effects.  However, when dependencies are not correctly specified, it can lead to unexpected re-renders and infinite loops.

## Bug Reproduction

1. Clone this repository.
2. Run `npm install` to install the necessary dependencies.
3. Run `npm start` to start the development server.
4. Observe the console output and the infinite loop in the browser.

## Solution

The solution involves correctly specifying the dependencies in the useEffect's dependency array. 

## Solution Explanation
The corrected code shows adding `count` to the dependency array. This ensures that the effect only runs when the `count` value changes, preventing the infinite loop.