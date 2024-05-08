"use strict";


//now we are defining the number which is to be guessed
const numbertobeguessed = Math.trunc(Math.random() * 20) + 1;

document.querySelector(".check").addEventListener("click", function () {
  // here the guess type is string

  const guess = Number(document.querySelector(".guess").value);

  if (!guess) {
    document.querySelector(".message").textContent = "No number!";
  } else if (guess === numbertobeguessed) {
    document.querySelector(".message").textContent = "Correct Number!";
  }
});
