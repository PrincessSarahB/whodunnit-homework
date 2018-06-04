Episode 1
var name = 'Bob';

var printName = function() {
  console.log('My name is ' + name );
};

printName();

<!-- This function will print out "My name is Bob" because Bob is assigned to the variable "name" -->

Episode 2

<!-- This function will return 3  -->
Episode 3
var myAnimals = ['Chickens', 'Cats', 'Rabbits'];

var listAnimals = function() {
  myAnimals = ['Ducks', 'Dogs', 'Lions'];
  for(var i=0;i<myAnimals.length; i++){
    console.log(i + ": " + myAnimals[i]);
  }
}

listAnimals();

<!-- This function will return the index number of each item: Ducks, Dogs and Lions because it is looping through the array within the function and then printing out the nunber assigned to "i" plus a colon plus the animals that are within the function as this overwrites the array outwith the function -->

Episode 4
var suspectOne = 'Ally';
var suspectTwo = 'Alan';
var suspectThree = 'Upul';
var suspectFour = 'Alistair';

var allSuspects = function() {
  var suspectThree = 'Colin'
  console.log('Suspects include: ' + suspectOne + ', ' + suspectTwo + ', ' + suspectThree + ', ' + suspectFour)
};

allSuspects();
console.log( 'Suspect three is:' + suspectThree );

<!-- Will print "Suspects include: Ally, Alan, Colin and Alistair", then "Suspect three is: Upul" because Colin overwrites Upul within the function, but outwith the function Upul is globally suspectThree -->

Episode 5
var detective = {
  name : 'Ace Ventura',
  pet : 'monkey'
};

var printName = function(detective) {
  return detective.name
};

var detectiveInfo = function() {
  detective['name'] = 'Poirot'
  return printName(detective);
};

console.log(detectiveInfo());

<!-- Will print out Poirot because Poirot is the name declared in the detectiveInfo function -->

Episode 6
var murderer = 'Rick';

var outerFunction = function() {
  var murderer = 'Morty';

  var innerFunction = function() {
    murderer = 'Jerry';
  }

  innerFunction();
}

outerFunction();
console.log('the murderer is ', murderer

<!-- Will print the murderer is Rick because the console log is using the global variable, not the ones local to the function -->

Episode 7 - Make up your own episode/s!
Make up your own episode which can be whatever you wish and the rest of the class will work out together what happened and what the output will be.
