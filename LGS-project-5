/*
Name: Gabriela Roberta Palma Milla
Date: November 25, 2026
Project: LGS Project 5 - Programiz test version
*/

// Function 1: request a number, validate, then check if prime.
function checkPrimeNumber() {
    const answer = prompt('Enter a non-negative whole number:');
    if (answer === null || !/^\d+$/.test(answer.trim())) {
        console.log('Input is invalid. Please enter 0 or a positive whole number.');
        return null;
    }
    const number = Number(answer);
    if (!Number.isSafeInteger(number)) {
        console.log('Input is invalid. Please enter a smaller whole number.');
        return null;
    }
    let isPrime = number >= 2;
    for (let divisor = 2; divisor * divisor <= number && isPrime; divisor++) {
        if (number % divisor === 0) isPrime = false;
    }
    console.log(`${number} is ${isPrime ? 'a prime number' : 'not a prime number'}.`);
    return number;
}

// Function 2: factorial of the same number.
function calculateFactorial(number) {
    let result = 1n;
    for (let i = 2; i <= number; i++) result *= BigInt(i);
    return result;
}

const number = checkPrimeNumber();
if (number !== null) {
    console.log(`Factorial of ${number} = ${calculateFactorial(number).toString()}`);
}
