import time
import random
import string

words = ["Sandy","SpongeBob","Squidward","Gary","Patrick","MrKrabs","MrsPuff","Pearl","Plankton","Karen","Mermaid"]
lives_visual_dict = {
        0: """
                ___________
               | /        | 
               |/       (xox)
               |         -|-
               |          |
               |
            """,
        1: """
                ___________
               | /        | 
               |/        ( )
               |         -|-
               |          |
               |
            """,
        2: """
                ___________
               | /        | 
               |/        ( )
               |          |
               |          |
               |
            """,
        3: """
                ___________
               | /        | 
               |/        ( )
               |          |
               |          
               |
            """,
        4: """
                ___________
               | /        | 
               |/        ( )
               |          
               |          
               |
            """,
        5: """
                ___________
               | /        | 
               |/        
               |          
               |          
               |
            """,
        6: """
                ___________
               | /        
               |/        
               |          
               |          
               |
            """,
        7: """
               |
               |
               |
               |
               |
            """,
        8: "",
    }
# Squidward's Quest for the Golden Clarinet
# IS 340
# Determined once and for all to prove to himself and everyone else that Squilliam Fancyson is a fraud and that he, 
# Squidward Tentacles, is the best clarinet player in Bikini Bottom, Squidward accepts Squilliam's challenge of retrieving 
# the golden clarinet, which can only be played by the musician with the best clarinet skills, from the Cave of Treble found at 
# the top of Mount Poseidon. You will travel alongside Squidward to retrieve the golden clarinet!

# There will be a total of 3 levels to complete. Each level will have a different objective.
# Level 1: Squidward will play a game of guess the correct door out of 3 doors.
# Level 2: Squidward will play a game of multiple choice questions.
# Level 3: Squidward will play a game of hangman.

# The game will end when Squidward reaches the golden clarinet.

# Main Menu
# The main menu will have the following options:
# 1. Play Game
# 3. Exit
def mainMenu():
    lives = 3
    print("-----------------------------------------------------")
    print("Welcome to Squidward's Quest for the Golden Clarinet!")
    print("-----------------------------------------------------")
    print("")
    print("Determined once and for all to prove to himself and everyone else that Squilliam Fancyson is a fraud and that he,")
    print("Squidward Tentacles, is the best clarinet player in Bikini Bottom, Squidward accepts Squilliam's challenge of retrieving")
    print("the golden clarinet, which can only be played by the musician with the best clarinet skills, from the Cave of Treble found at")
    print("the top of Mount Poseidon. You will travel alongside Squidward to retrieve the golden clarinet!")
    print("")
    print("1. Play Game")
    print("")
    print("2. Exit")
    print("")
    choice = input("Enter your choice: ")
    if choice == "1":
        # Levels
        level1(lives)
        mainMenu()
    elif choice == "2":
        exit()
    else:
        print("Invalid choice. Please try again.")
        mainMenu()
        
# Level 1
# Squidward will play a game of guess the correct door out of 3 doors.
# The game will have 3 doors, 2 of which will have monsters behind it and 1 will open a path to the top of Mount Poseidon.
# If Squidward guesses the wrong door, he will lose a life.
# If Squidward guesses the correct door, he will move on to the next level.
# If Squidward loses all 3 lives, the game will end.
def level1(lives):
    print("")
    print("")
    print("Level 1: Guess the correct door")
    print("")
    print("You will be given 3 doors to choose from. One of the doors will lead you to the top of Mount Poseidon.")
    print("")
    print("The other two doors will have a monster behind it. You will lose a life if you choose the wrong door.")
    print("")
    print("You will have 3 lives to complete this level.")
    print("------------------------------------------------------------------------------------------------------")
    print("Good luck!")
    print("------------------------------------------------------------------------------------------------------")
    print("")
    doors = {"Door 1": "Wrong", "Door 2": "Wrong", "Door 3": "Wrong"}
    correctDoor = random.choice(list(doors.keys()))
    doors[correctDoor] = "Correct"
    while lives > 0:
        print("You have", lives, "lives left.")
        print("")
        print("1. Door 1")
        print("")
        print("2. Door 2")
        print("")
        print("3. Door 3")
        print("")
        choice = input("Enter your choice: ")
        # Dictionary of doors and one random door is selected as the correct door while the rest are wrong doors
        if choice == "1":
            if doors["Door 1"] == "Correct":
                print("Congratulations you've successfully opened the correct door.")
                print("You continue on your journey and find yourself infront of a path that leads into a dark seaweed forest.")
                level2(lives)
                break
            else:
                print("You have chosen door 1.")
                print("You have been hurt by the Alaskan Bull Worm.")
                lives = lives - 1
                print("You have", lives, "lives left.")
                print("")
        elif choice == "2":
            if doors["Door 2"] == "Correct":
                print("Congratulations you've successfully opened the correct door.")
                print("You continue on your journey and find yourself infront of a path that leads into a dark seaweed forest.")
                level2(lives)
                break
            else:
                print("You have chosen door 2.")
                print("You have been injured by the Dirty Bubble.")
                lives = lives - 1
                print("You have", lives, "lives left.")
                print("")
        elif choice == "3":
            if doors["Door 3"] == "Correct":
                print("Congratulations you've successfully opened the correct door.")
                print("You continue on your journey and find yourself infront of a path that leads into a dark seaweed forest.")
                level2(lives)
                break
            else:
                print("You have chosen door 3.")
                print("You were stung by the Giant Jellyfish.")
                lives = lives - 1
                print("You have", lives, "lives left.")
                print("")
        else:
            print("Invalid choice. Please try again.")
    if lives == 0:
        print("You have lost all your lives. Game over.")
        mainMenu()
    
"""
Created on Tue Nov 22 20:44:44 2022
@author: dylanmbecker
"""
def level2(lives):
    time.sleep(1)
    print("As you follow the path you sense you are being watched and hear coral branches cracking all around.")
    time.sleep(1) # To pass the bandit you must answer his question
    print("You hear footsteps behind you and you spin around with fear ... no ones there.")
    time.sleep(1)
    print("You turn around to continue on the path, but just as you take your next step you hear a noise.")
    time.sleep(1)
    print("Blackfin the Barracuda Bandit jumps out and blocks you from proceeding.")
    time.sleep(1)
    print('Blackfin: "You will go no further until you can beat me in a duel to the death."')
    time.sleep(1)
    print('Squidward: "Duel?!?"')
    time.sleep(1)
    print('Blackfin: "Yes, but do not fear. This is a battle of chance. Those who have the favor of Poseidon will triumph."')
    time.sleep(1)

    # Ask user for permission to continue
    continuation = True
    while continuation:
        advance = input("Do you wish to continue? 'Yes' or 'No':  ").upper()
        print("_______________________________________________________________________________\n")
        if advance == "YES":
            continuation = False # Leave the loop
            print("Okay, you accept the duel.\n")
            print("Choose your attack wisely. For every wrong mistake you will lose a life point.")
            time.sleep(1)
        elif advance == "NO":
            print("You don't seem ready to take on this challenger.")
            print("You walk out of the coral forest, down the ravine, and hop into your bathtub.")
            time.sleep(1)
            print("Game Over")
            # Option to play again
            playAgain = input("Would you like to play again? 'Yes' or 'No':  ").upper()
            if playAgain == "YES":
                mainMenu()
            elif playAgain == "NO":
                print("Goodbye")
                exit()
            else:
                print("Invalid choice. Please try again.")
                playAgain()
        else:
            print("That is not a valid response!")

    print("Blackfin: This duel will consist of 3 choices: Rock, Paper, Scissors")
    time.sleep(1)
    print("Blackfin: Best of Three")
    time.sleep(1)
    print("Blackfin: Ready?")
    time.sleep(1)
    print("Blackfin: 3")
    time.sleep(.5)
    print("Blackfin: 2")
    time.sleep(.5)
    print("Blackfin: 1")
    time.sleep(.5)
    print("Blackfin: GO!")
    
    # Rock Paper Scissors
    # Squidward will have 3 lives to complete this level.
    # If Squidward loses all 3 lives, the game will end.
    SquidwardScore = 0
    BlackFinScore = 0
    while lives > 0:
        if BlackFinScore > 2:
            print("BlackFin The Bandit has won the game and you lost a life.")
            lives -= 1
            if lives == 0:
                print("You have lost all your lives.")
                print("Game Over!")
                mainMenu()
            print("You now have %d lives\n" %(lives))
            time.sleep(1)
            print("BlackFin: You have lost this round, but I will play you again.")
            print("BlackFin: Ready?")
        elif SquidwardScore > 2:
            print("Congratulations, you have defeated Blackfin the Barracuda Bandit in combat! \n")
            print("As blackfin falls to the ground, he drops a health potion.")
            print("You pick it up and drink it, gaining +5 health.")
            lives += 5
            print("You now have %d lives\n" %(lives))
            print("You continue on your journey and reach level 3.")
            level3(lives)
            break
        results = rockPaperScissors(0, 0)
        BlackFinScore = results[0]
        print("BlackFin Score: %d" %(BlackFinScore))
        SquidwardScore = results[1]
        print("Squidward Score: %d" %(SquidwardScore))

def rockPaperScissors(BlackFinScore, SquidwardScore):
    while (BlackFinScore < 3) and (SquidwardScore < 3):
        #user inputs
        user_action = input("Enter a choice (rock, paper, scissors): ").lower()
        #monster actions
        possible_actions = ["rock", "paper", "scissors"]
        monster_action = random.choice(possible_actions)
        #Actions from both
        print(f"\nYou chose {user_action}, Blackfin chose {monster_action}.")
        #if/else statements for the game
        if user_action == monster_action:
            print(f"Both players selected {user_action}. It's a tie!")
            print("Score: You %d, BlackFin %d \n" %(SquidwardScore, BlackFinScore))
        elif user_action == "rock":
            if monster_action == "scissors":
                SquidwardScore += 1
                print("Rock smashes scissors! You win!\n")
                print("Score: You %d, BlackFin %d \n" %(SquidwardScore, BlackFinScore))
            else:
                BlackFinScore += 1
                print("Paper covers rock! Blackfin gains a point.")
                print("Score: You %d, BlackFin %d \n" %(SquidwardScore, BlackFinScore))
        elif user_action == "paper":
            if monster_action == "rock":
                SquidwardScore += 1
                print("Paper covers rock! You win!\n")
                print("Score: You %d, BlackFin %d \n" %(SquidwardScore, BlackFinScore))
            else:
                BlackFinScore += 1
                print("Scissors cuts paper! Blackfin gains a point.")
                print("Score: You %d, BlackFin %d \n" %(SquidwardScore, BlackFinScore))
        elif user_action == "scissors":
            if monster_action == "paper":
                SquidwardScore += 1
                print("Scissors cuts paper! You win!\n")
                print("Score: You %d, BlackFin %d \n" %(SquidwardScore, BlackFinScore))
            else:
                BlackFinScore += 1
                print("Rock smashes scissors! Blackfin gains a point.")
                print("Score: You %d, BlackFin %d \n" %(SquidwardScore, BlackFinScore))
        else :
            print("Invalid input! You have not entered rock, paper or scissors, try again.")
            print("Score: You %d, BlackFin %d \n" %(SquidwardScore, BlackFinScore))

    print("Final Scores: You %d, BlackFin %d \n" %(SquidwardScore, BlackFinScore))
    if SquidwardScore > BlackFinScore:
        print("You win!")
        return BlackFinScore, SquidwardScore
    elif SquidwardScore < BlackFinScore:
        print("Blackfin wins!")
        return BlackFinScore, SquidwardScore
    
# Level 3
# Hangman - Vincent Fu
# Squidward will face the final trial of receiving the golden clarinet from the Cave of Treble by challenging the cave directly.
def level3(lives):
    print("Cave of Treble")
    print("_______________________________________________________________________________\n")
    time.sleep(1)
    print("You have entered the Cave of Treble. You see a large, dark, and ominous cave.")
    time.sleep(1)
    print("You hear a faint voice coming from the cave.")
    time.sleep(1)
    print("Voice: Hello, I am the Cave of Treble. I will test your knowledge.")
    time.sleep(1)
    print("Voice: If you can guess the character I am thinking of, you will be rewarded with the golden clarinet.")
    time.sleep(1)
    print("Voice: If you cannot, you will be punished.")
    time.sleep(1)
    print("Voice: Are you ready?")
    time.sleep(1)
    print("Voice: 3")
    time.sleep(.5)
    print("Voice: 2")
    time.sleep(.5)
    print("Voice: 1")
    time.sleep(.5)
    print("Voice: GO!")
    time.sleep(1)
    
    word = get_valid_word(words)
    word_letters = set(word)  # Letters in the word
    alphabet = set(string.ascii_uppercase)
    used_letters = set()  # What the user has guessed

    # Getting user input
    while len(word_letters) > 0 and lives > 0:
        # Letters used
        # ' '.join(['a', 'b', 'cd']) --> 'a b cd'
        print('You have', lives, 'lives left and you have used these letters: ', ' '.join(used_letters))

        # What current word is (ie W - R D)
        word_list = [letter if letter in used_letters else '-' for letter in word]
        print(lives_visual_dict[lives])
        print('Current character: ', ' '.join(word_list))

        user_letter = input('Guess a letter: ').upper()
        if user_letter in alphabet - used_letters:
            used_letters.add(user_letter)
            if user_letter in word_letters:
                word_letters.remove(user_letter)
                print('')

            else:
                lives = lives - 1  # Takes away a life if wrong
                print('\nYour letter,', user_letter, 'is not in the word.')

        elif user_letter in used_letters:
            print('\nYou have already used that letter. Guess another letter.')

        else:
            print('\nThat is not a valid letter.')

    # Gets here when len(word_letters) == 0 OR when lives == 0
    if lives == 0:
        print(lives_visual_dict[lives])
        print('You died, sorry. The character was', word)
        return lives
    else:
        print('Voice: Congratulations! You have guessed the word', word, '!')
        print('You have retrieved the golden clarinet.')
        print("Congratulations for finishing the game!")
        
def get_valid_word(words):
    word = random.choice(words)  # Randomly chooses something from the list
    print('Voice: I am thinking of a character that is', len(word), 'letters long.')
    while '-' in word or ' ' in word:
        word = random.choice(words)
        
    return word.upper()

# Starts the Game
mainMenu()
