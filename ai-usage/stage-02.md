## Tools- Google Gemini
## Key requests
- ### 1. Asked: Why the Vite server wasn't starting.
- Got: Explained that Vite created a new subfolder, so I needed to run `cd app` before `npm run dev`.
- Changed or rejected: Applied successfully.

- ### 2. Asked: How to fix the "ReactDOMClient.createRoot()" error in the console.
- Got: Pointed out that I accidentally duplicated the React initialization block and misplaced imports while copying from the lab. 
- Changed or rejected: Cleaned up `main.jsx` and the error disappeared.

## What I learned / what did not work
Running `npm run dev` in the main folder did not work; I learned to navigate into the Vite subfolder first. I also learned that JavaScript `import` statements must always sit at the top of the file, and React's `createRoot` must only be called once to avoid rendering errors.