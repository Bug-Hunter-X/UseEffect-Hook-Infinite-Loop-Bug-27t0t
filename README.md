# React useEffect Hook Infinite Loop Bug
This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by a missing dependency array.

## Bug Description
The `useEffect` hook is used to perform side effects after a component renders. If a dependency array is not provided, the effect runs on every render, potentially creating an infinite loop.  In this case, the `console.log` statement inside the effect causes a re-render which in turn leads to the effect running again, and so on.