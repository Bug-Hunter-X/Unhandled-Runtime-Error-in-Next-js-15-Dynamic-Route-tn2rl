# Unhandled Runtime Error in Next.js 15 Dynamic Route

This repository demonstrates an unhandled runtime error that can occur in Next.js 15 when accessing undefined variables within a page component.  The error is not caught by the default Next.js error boundary, leading to a crash of the page.

## Problem

Accessing a variable that is not defined in your component's scope will result in a runtime error. In Next.js 15, if this happens in a dynamic route or page component, the error isn't gracefully handled and may lead to a broken user experience.

## Solution

The solution is to implement proper error handling. Use try...catch blocks or conditional checks before attempting to access potentially undefined variables to avoid unexpected crashes and display meaningful error messages to users.