# javascript-test-0002-final-13941-omkar
# Final Project Assignment - This repository contains the complete final project code and documentation.


const ROWS = 5;

for (let i = 0; i < ROWS; i++) {
    let row = "";
    // spacing
    for (let space = 0; space < i; space++) {
        row += " ";
    }
    let length = ROWS - i;
    for (let j = 0; j < length; j++) {
        if (j === 0 || j === length - 1) {
            row += "1 ";
        } 
        else if (i === 0 && j === 2) {
            row += "6 ";
        } 
        else {
            row += (ROWS - i - 1) + " ";
        }
    }
    console.log(row.trim());
}
