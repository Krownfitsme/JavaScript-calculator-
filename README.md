# JavaScript-calculator-// Function to perform addition
function add(a, b) {
  return a + b;
}

// Function to perform subtraction
function subtract(a, b) {
  return a - b;
}

// Function to perform multiplication
function multiply(a, b) {
  return a * b;
}

// Function to perform division
function divide(a, b) {
  if (b === 0) {
    return "Error: Cannot divide by zero";
  }
  return a / b;
}

// Function to handle user input and perform calculation
function calculate() {
  var operator = prompt("Enter an operator (+, -, *, /):");
  var num1 = parseFloat(prompt("Enter the first number:"));
  var num2 = parseFloat(prompt("Enter the second number:"));
  var result;

  switch (operator) {
    case "+":
      result = add(num1, num2);
      break;
    case "-":
      result = subtract(num1, num2);
      break;
    case "*":
      result = multiply(num1, num2);
      break;
    case "/":
      result = divide(num1, num2);
      break;
    default:
      result = "Invalid operator";
  }

  console.log("Result: " + result);
}

// Call the calculate function to start the calculator
calculate();
