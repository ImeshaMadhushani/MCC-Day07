# React Parent-Child Communication 
# 2020ICT90

## Project Overview
This is a simple React application that demonstrates parent-child communication using state and props. The parent component (`App.js`) passes a function as a prop to the child component (`Childcom.js`), and the child component calls this function to send data back to the parent. The parent then updates its state based on the data received from the child.

## Files
- `App.js`: The parent component that manages the state and passes a function to the child component.
- `Childcom.js`: The child component that calls the function passed down by the parent to send data back.
- `App.css`: Basic styling for the components.
- `package.json`: Contains project dependencies and configuration.

## Key Concepts Covered
1. **State Management with `useState`**: The parent component manages a piece of state (`childname`) that gets updated based on input from the child component.
2. **Props and Functions**: The parent passes a function (`receiveName`) to the child component through props, allowing the child to update the parent's state.
3. **Functional Components**: Both the parent and child components are functional components, which are a core part of modern React development.

## How It Works
1. The `App.js` component renders the `Childcom` component and passes a function `receiveName` as a prop (`setfun`).
2. The `Childcom` component immediately calls the `setfun` function when it is rendered, passing the string `"My Name is Bob"` to the parent.
3. The `receiveName` function updates the parent's state (`childname`) with the value passed from the child.
4. The parent component then renders the updated state inside a `<p>` tag, showing the message: "Parent: My child said: My Name is Bob".

## How to Run
1. Clone the repository to your local machine.
2. Navigate to the project folder and run `npm install` to install all the dependencies.
3. Start the development server by running `npm start`.
4. Open your browser and go to `http://localhost:3000` to see the application in action.

## Output
![Screenshot 2024-11-21 204515](https://github.com/user-attachments/assets/12dcdc7a-2886-428d-9321-956902d722dc)
