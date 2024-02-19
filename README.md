# CODSOFT
This code creates a simple calculator with basic arithmetic operations. 
that using eval for calculation can have security implications, and it is generally advisable to use a safer method
The provided code is a basic implementation of a calculator using HTML, CSS, and JavaScript. Let me break down the key components of the project:

1.HTML Structure:
   
The HTML structure is straightforward, containing a <div> with the id "calculator" that holds the calculator interface.
An <input> element with the id "display" is used to show the current input and results. It is disabled to prevent user input.

2.CSS Styling:

The CSS is minimal and focused on styling the calculator for a simple and clean appearance.
Flexbox is used to center the calculator on the page.
Buttons and input fields have basic styling to make them visually appealing.

3.JavaScript Functions:

Three main JavaScript functions are defined in the <script> section:
appendToDisplay(value): This function appends the provided value to the display input field when a number or operator button is clicked.
calculate(): This function evaluates the expression in the display input field using eval() when the "=" button is clicked. It handles potential errors and displays "Error" if encountered.
clearDisplay(): This function clears the content of the display input field when the "C" button is clicked.

4.Button Click Events:

Each button on the calculator has an onclick attribute that calls the corresponding JavaScript function when clicked.
Numeric buttons (0-9), decimal point (.), and arithmetic operation buttons (+, -, *, /) append their respective values to the display.
The "=" button triggers the calculation, and the "C" button clears the display.

5.Eval Function:

The use of eval() for calculation simplifies the code but comes with security risks. In a real-world scenario, it is recommended to use a safer method, like parsing and evaluating the expression manually, to avoid potential security vulnerabilities associated with eval().

6.Error Handling:

The try-catch block is used to handle potential errors during the evaluation of the expression. If an error occurs, the display shows "Error."
