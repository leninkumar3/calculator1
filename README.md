function calculator(a, b, operator) {
    let result;
    switch (operator) {
        case '+':
            result = a + b;
            break;
        case '-':
            result = a - b;
            break;
        case '*':
            result = a * b;
            break;
        case '/':
            result = a / b;
            break;
        case '^':
            result = Math.pow(a, b);
            break;
    }
    return result;
}

function main() {
    let a, b;
    let result;
    let choice;
    let operator;
    do {
        console.log("Enter the numbers:");
        a = parseInt(prompt("Enter the first number:"));
        b = parseInt(prompt("Enter the second number:"));
        operator = prompt("Enter the operation to perform (+, -, *, /, ^):");
        result = calculator(a, b, operator);
        console.log("Result is:", result);
        choice = parseInt(prompt("Press 1 to continue, press 0 to stop:"));
        if (choice === 0) {
            console.log("Exiting...");
        }
    } while (choice !== 0);
}

main();
# calculator1
