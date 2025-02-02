# Next.js 15 Undefined Variable Bug

This repository demonstrates a common runtime error in Next.js 15 applications: referencing an undefined variable within a functional component.  The error is specifically triggered when navigating to the '/about' page.

## Bug Description
The `about.js` file attempts to render the value of a variable (`myVar`) that has not been defined. This results in a runtime error.

## How to Reproduce
1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm run dev` to start the Next.js development server.
4. Navigate to `http://localhost:3000/about`.

You should see a runtime error in your browser's console.

## Solution
The solution is to either define the `myVar` variable correctly within the `About` component or, if the variable should come from elsewhere (props, API call, etc.), make sure the data is properly fetched and passed to the component before attempting to use it. The solution is provided in `aboutSolution.js`
