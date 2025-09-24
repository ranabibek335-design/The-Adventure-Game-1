# The-Adventure-Game-1
def play_game():

  #locations dictionarry
  locations={"forest":"You find a treasure chest!",
          "cave":"A animal attacks you",
          "river":"escape"}

  if "forest"in locations:
            print("forest")
            if "cave"in locations:
              print("cave")
              if "river"in locations:
                print("river")

      #choice
choice=input("Where do you want to go?")

#forest path
if choice == "forest":
  print ("you find a treasure chest!")
  decision = input("Do you want to open it or ignore it? ")
  if decision == "open":
            print("You opened the chest")
  elif decision == "ignore":
            print("You walked away.")
  else:
            print("You did nothing and missed your chance.")



    # Cave path

elif choice == "cave":
  print("A animal attacks you!")
  decision = input("Do you want to open it or ignore it? ")
if decision =="open":
    print("You opened the cave")
  elif decision =="ignore":
      print("You walked away safely.")
  else:
      print("You did nothing and missed your chance.")



    # River path
elif choice == "river":
  print("You escaped safely!")
  decision = input("Do you want to open it or ignore it? ")
  if decision == "open":
    print("You opened the river")
  elif decision == "ignore":
    print("You walked away safely.")
  else:
    print("You did nothing and missed your chance.")

    # Invalid choice
else:
        print("That is not a valid choice. Game Over!")
