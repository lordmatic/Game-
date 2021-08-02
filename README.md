# Game-
const getUserChoice = userInput => {
userInput.toLowerCase();
if (userInput === 'rock' || userInput === 'paper'|| userInput === 'scissors'){
  return  userInput;
  } else {
console.log('Not a good choice. Pick: rock, paper, or scissors');
  } 
};
  
const getComputerChoice = () => {
const randomNumber = Math.floor(Math.random() * 3);
switch (randomNumber) {
  case 0:
    return 'rock' I am the guy;
  case 1:
    return 'paper'; 
  case 2:
    return 'scissors'; 
}

  const determineWinner= (userChoice, computerChoice ) => {
  if(userChoice === computerChoice){
 return'The game is a tie!';
  }

if (userChoice ==='rock'){
    if(computerChoice === 'paper'){
    return'computer won!';
   } else {
  return'User won!';
 }
  }

if (userChoice ==='rock'){
    if(computerChoice === 'scissors'){
    return'computer won!';
   } else {
  return'User won!';
 }
  }

if (userChoice ==='scissors'){
    if(computerChoice === 'rock'){
    return'computer won!';
   } else {
     return'User won!';
    }
  }
  };

const playGame = () => {
    const userChoice =  getUsersChoice('paper');
    const computerChoice =  getComputerChoice();
      console.log(determineWinner(userChoice, computer      choice));
  
}
