# Unexpected Re-renders in React useEffect Hook

This repository demonstrates a common issue encountered when using the `useEffect` hook in React: unexpected re-renders due to missing dependencies in the dependency array.

## Problem

The provided `MyComponent` uses `useEffect` to log the current `count` to the console.  However, the dependency array `[count]` is correctly declared and this prevents infinite renders. 

## Solution

The solution involves ensuring that the dependency array includes all values from the component's scope that the effect relies on. In this case, `count` is correctly added to the dependency array.

## How to Run

1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server. 
