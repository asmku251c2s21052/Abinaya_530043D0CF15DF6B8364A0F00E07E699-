"""Implement a class called player that represent a cricket player. 
The Player class should have a 
method called play() which prints "The player is playing cricket". Derive two classes, Batsman and Bowler, from the player class. override the play() method in each derived classes to print "The batsman 
is batting" and "The bowler is bowling", respectively. Write a program to create objects of both the 
Batsman and bowler classes and call the play() method for each object."""


#define the base class Player
class Player:
    def play(self):
        print("The player is playing cricket.")

#define the derived class Batsman
class Batsman(Player):
    def play(self):
        print("The batsman is batting.")

#define the derived class Bowler
class Bowler(Player):
    def play(self):
        print("The bowler is bowling.")
      
#create objects of Batsman and Bowler classes
batsman = Batsman()
bowler = Bowler()

#call the play() method for each object
batsman.play()
bowler.play()