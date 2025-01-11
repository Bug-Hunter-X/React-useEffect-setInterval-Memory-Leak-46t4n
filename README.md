# React useEffect setInterval Memory Leak

This repository demonstrates a common error in React applications: memory leaks caused by the improper use of `setInterval` within the `useEffect` hook. 

The `bug.js` file contains a component that uses `setInterval` to update a counter every second.  However, it lacks the necessary cleanup function to stop the interval when the component unmounts. This leads to a memory leak as the interval continues to run even after the component is no longer in use.

The `bugSolution.js` file shows the corrected version of the component with a proper cleanup function to prevent memory leaks.