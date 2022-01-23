# Convert-Text-to-Whale-Song-
This is another project from Codecademy where you convert text to whale song!

// Example input sentence, should output to 'EEEEIAAOEEEEEEUUO'
const input = 'Here is a random sentence uh wow.';
const vowels = ['a', 'e', 'i', 'o', 'u'];
let resultArray = [];

// Pulls every letter from the input and compares it to the vowels array.
for (let i = 0; i < input.length; i++) {
  // Stores captured vowels from input to resultArray
  for (let j = 0; j < vowels.length; j++) {
    if (input[i] === vowels[j]) {
      resultArray.push(input[i]);
    }
    // Doubles vowels e and u and stores them to resultArray
  } if (input[i] === 'e' || input[i] === 'u') {
      resultArray.push(input[i]);
    }
}

// Capitalizes and concatinates resultArray's content
console.log(resultArray.join('').toUpperCase());
