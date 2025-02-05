# React useEffect Dependency Array Bug

This repository demonstrates a common bug in React's `useEffect` hook related to the dependency array. The `useEffect` hook's functionality is incorrectly implemented, resulting in an unexpected behavior. The solution shows how to correctly manage dependencies in `useEffect` to fix the issue.

## Bug Description

The bug lies in the conditional statement within the `useEffect` hook. The condition `count > 10` is checked only once when the component mounts. Subsequent changes to the `count` state variable do not trigger the conditional statement as expected, due to the incorrect use of the dependency array. This can lead to unexpected behavior and logic errors. The console log will only run once at initial render, not every time count exceeds 10.

## Solution

The solution involves modifying the conditional statement and ensuring the correct dependencies are included in the `useEffect`'s dependency array.