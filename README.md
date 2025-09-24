# Start the game
def play_game():
    # Ask player name
    name = input("What is your name? ")

    # Show choices
    print("Choose a location:")
    print("forest")
    print("cave")
    print("river")

    choice = input("Where do you want to go? ")

    # Forest path
    if choice == "forest":
        print("You see a treasure chest!")
        decision = input("Do you want to open it or ignore it? ")

        if decision == "open":
            print("You opened the chest and found gold!")
        elif decision == "ignore":
            print("You walked away safely.")
        else:
            print("You did nothing and missed your chance.")

    # Cave path
    elif choice == "cave":
        print("A wild animal attacks you!")

    # River path
    elif choice == "river":
        print("You found a boat and escaped safely!")

    # Invalid choice
    else:
        print("That is not a valid choice. Game Over!")



