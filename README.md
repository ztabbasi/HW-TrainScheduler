# HW-TrainScheduler

Train Scheduler : The page allows you to add new trains with their destinations, start times and frequencies.  It then add the train to the bulleting and gives the train name, destination, frequency, next arrival time and minutes to the next arrival

Link to the site
Crystal Game

Images
Picture

Technologies used
HTML CSS Javascript Jquery

code snippets
Test which crystal was clicked and add based on the crystal's hidden value and check if still below total

var crystalValue = ($(this).attr("data-crystalvalue"));
crystalValue = parseInt(crystalValue);
// We then add the crystalValue to the user's "counter" which is a global variable.
// Every click, from every crystal adds to the global counter.
counter += crystalValue;

// All of the same game win-lose logic applies. So the rest remains unchanged.
//alert("New score: " + counter);
$("#score").text(counter);
   
if (counter === targetNumber) {
  wins++;
  $("#wins").text(wins);
  counter=0;
  resetGame();
}

else if (counter >= targetNumber) {
  losses++;
  $("#losses").text(losses);
  counter=0;
  resetGame();
}
Author
Zia Abbasi

License
Standard MIT License
