# HW-TrainScheduler

Train Scheduler : The page allows you to add new trains with their destinations, start times and frequencies.  It then add the train to the bulleting and gives the train name, destination, frequency, next arrival time and minutes to the next arrival

# Link to the site

[Train Scheduler Game](https://ztabbasi.github.io/HW-TrainScheduler/)

# Images

![Picture](assets/images/trainScheduler.PNG)

# Technologies used

HTML,
CSS,
Javascript
and Firebase



# code snippets

The code snipet below initializes the Firebase database.  It then creates a "submit" button to add a train
using train name, destination, first train of day and frequency as inputs. It then uses a temporary train
object to store that information.

// 1. Initialize Firebase
var config = {
    apiKey: "AIzaSyCER01ei_LIHw6BEh2tz_MaglCti50I_4c",
    authDomain: "custom-no-share.firebaseapp.com",
    databaseURL: "https://custom-no-share.firebaseio.com",
    projectId: "custom-no-share",
    storageBucket: "custom-no-share.appspot.com",
    messagingSenderId: "708411308872"
  };
  firebase.initializeApp(config);
  
  var database = firebase.database();
  
  // 2. Button for adding Train
  $("#add-train-btn").on("click", function(event) {
    event.preventDefault();
  
    // Grabs user input
    var trainName = $("#train-name-input").val().trim();
    var destination = $("#destination-input").val().trim();
    var firstTrain = $("#first-train-input").val().trim();
    var frequency = $("#frequency-input").val().trim();
  
    // Creates local "temporary" object for holding employee data
    var newTrain = {
      name: trainName,
      dest: destination,
      first: firstTrain,
      freq: frequency
    };


# Author 
Zia Abbasi

# License
Standard MIT License
