# React Router Dom Wildcard Route Issue

This repository demonstrates a problem with React Router Dom v6 where nested routes interfere with the expected behavior of the wildcard route (`*`). The wildcard route should only match routes not matched by other routes. However, this is not the case when nested routes are used.

## Problem

The issue occurs when using nested routes in combination with a wildcard route. In this case, the wildcard route incorrectly intercepts any route that is not explicitly defined. 

## Solution

The proposed solution is to use a different approach for handling unmatched routes. This solution can involve modifying how the routes are defined or adding a fallback route after all other specific routes have been defined.

## How to Reproduce

1. Clone this repository.
2. Install dependencies using `npm install`.
3. Run the application using `npm start`.
4. Observe the behavior of the application when navigating to different routes. Note how the wildcard route is triggered unexpectedly.

## Setup

1. Ensure you have Node.js and npm (or yarn) installed on your system. 
2. Install the React Router Dom package using `npm install react-router-dom@6` (or yarn add react-router-dom@6).