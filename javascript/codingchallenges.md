## remove vowels
### create variable to hold function and string
function disemvowel(string){
### create variable to hold split string
  let charArray = string.split("");
### for loop x equals zero, is less than length of string, and passes on to next string
  for (let x = 0; x < string.length; x++) {
### variable to hold if statement
    let char = string[x]
### if char equals a vowel
    if (char == "a" || char == "e" || char == "i" || char == "o" || char == "u"){
### return empty string
      charArray[x] = ""
    }
  }
### rejoin the single letters strings into a word string
  return charArray.join('')
  
 }

## remove vowels shorter
function shortcut(string){
### return a replaced empty string for vowels
  return string.replace(/[aeiou]/g,'')
}

## calculate blank pages for classmante
function paperwork(n, m) {
  if(n < 0 || m < 0){
    return 0
  } else {
   return n * m
  }
}

## repeat string (s), (n) number of times
function repeatStr (n, s) {
## return repeat function
  return s.repeat(n)
}

## find the remainder
function remainder(a, b){
  if(a > b){
    return a % b
  } else {
    return b % a
  }
}

## find the remainder (ternary)
function remainder(a, b){
  return a > b ? a % b : b % a;
}

## making six toast
function sixToast(num) {
## Math.abs returns the absolute value of a number
  return Math.abs(num-6)
}

## Sentence Smash (return seperate words in an array as a sentence)
function smash (words) {
    return words.join(' ')
}

## write a function that converts the input string to uppercase
function makeUpperCase(str) {
  return str.toUpperCase()
}

## rock paper scissors (answer 1)
const rps = (p1, p2) => {
  if (p1 == p2)
    return 'Draw!';
    
   if (p1 == 'rock' && p2 == 'scissors') 
     return 'Player 1 won!'
   else if (p1 == 'scissors' && p2 == 'paper') 
     return 'Player 1 won!'
   else if (p1 == 'paper' && p2 == 'rock') 
     return 'Player 1 won!'
   else
     return 'Player 2 won!';
};

## rock paper scissors (answer 2)
const rps = (p1, p2) => {
  if (p1 === p2) return "Draw!";
  var rules = {rock: "scissors", paper: "rock", scissors: "paper"};
  if (p2 === rules[p1]) {
    return "Player 1 won!";
  }
  else {
    return "Player 2 won!";
  }
};

## Calculating Final Grade
function finalGrade (exam, projects) {
  if (exam > 90 || projects > 10) return 100;
  else if (exam > 75 && projects >= 5) return 90;
  else if (exam > 50 && projects >= 2) return 75;
  else return 0;
}

## Duty Free 
function dutyFree(normPrice, discount, hol){
  return(Math.floor(hol / normPrice / discount * 100))
}

## Well of ideas
const well = x => {
  const good_count = x.filter(x => x == 'good').length;
  return good_count < 1 ? 'Fail!' : 
         good_count < 3 ? 'Publish!' : 'I smell a series!';
}

## Twice as old 
function twiceAsOld(dadYearsOld, sonYearsOld) {
  return Math.abs(dadYearsOld - 2 * sonYearsOld);
}

## DNA to RNA 
function DNAtoRNA(dna){
  return dna.replace(/T/g, 'U');
}
