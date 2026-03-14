
const ROWS = 5;

for (let i = ROWS - 1; i >= 0; i--) {
    let row = "";
    for (let space = 0; space < ROWS - 1 - i; space++) {
        row += " ";
    }
    let num = 1;
    for (let j = 0; j <= i; j++) {
        row += num + " ";
        num = num * (i - j) / (j + 1);
    }
    console.log(row.trim());
}
