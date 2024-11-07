# React---Changing-Complex-State

# Full Name Form App

This is a simple React app that allows users to enter their first and last names in a form. The app dynamically displays the full name as the user types, demonstrating controlled components and state management in React.

**git clone https://github.com/jbolan12/React---Changing-Complex-State.git**

## Features

- **Real-time Name Update**: The entered first and last names are displayed in real-time as the user types.
- **Controlled Components**: The app demonstrates the use of controlled components in React by managing the input fields' values through state.
- **Spread Operator Usage**: Uses the spread operator to handle and update object state properties in React.

## Code Explanation

- **State Management**:
  - The `fullName` state is an object with two properties: `fName` and `lName`.
  - `setFullName` updates the state, using the spread operator to merge the previous state and the new input field value.
- **Event Handling**:
  - `handleChange` destructures the `name` and `value` properties from the event target to identify which input is being changed and updates the state accordingly.
 
## Dependencies
- React: 18.3.1
- React-DOM: 18.3.1
- React-Scripts 5.0.1

## License
This project is licensed under the MIT License. See the LICENSE file for details.

### Code Example

```javascript
const [fullName, setFullName] = useState({
  fName: "",
  lName: "",
});

function handleChange(event) {
  const { name, value } = ev
