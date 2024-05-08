#constants
Rock = 1
Paper = 2
Scissors = 3

#Define the main function
def main():

    #set control loop
    keep_going = 'Y'


    #set counter to zero
    computer_wins = 0
    player_wins = 0
    tie_score = 0

    #call display message
    display_message()

    while keep_going == 'y' or keep_going == 'Y':

        play_game()


        #prompt user to keep going
        keep_going = input('would you like to play again? (Y for Yes): ')

    print('The computer won', computer_wins, 'times')
    print('The player won', player_wins, 'times')
    print('There were', tie_score, 'tie scores')

def play_game():

    #get random input
    computer = get_random()

    #get the players input
    play = get_play()

    #validate input
    if play == '1' or play == '2' or play == '3':
        play == True
    else:
        play == False
        print('Error: Invalid Entry')
        play = input('Please enter 1 for Rock, 2 for Paper, or 3 for Scissors: ')

    if play == computer:
        print('Tie Score, Please try again')
        tie_score += 1

    else:
        get_score(computer, play)

    print('The computer chose:', computer)
    print('The player chose: ', play)


#define display message
def display_message():
    print('Welcome to Rock Paper Scissors, a game of chance to see who will')
    print('outsmart the other. This game is Man VS Computer.')
    print('The program will select a random integer and then ask you for an integer')
    print('1 for Rock 2 for paper or 3 for Scissors. The program will then tell')
    print('you who won the game.')
    print('GOOD LUCK!')
    print
    print

def get_random():
    import random

    #generate random int
    computer = random.randint(1, 3)
    return computer


def get_play():
    #prompt user to enter an integer 1, 2, or 3
    play = input('Select 1 for Rock, 2 for Paper, or 3 for Scissors: ')
    return play

def get_score(computer, play):

    if computer == 1 and play == 2:
        score = 'player wins'
        print('Paper covers Rock, Player Wins')
        #player wins
        player_wins += 1

    elif computer == 1 and play == 3:
        score = 'computer wins'
        print('Scissors cut Paper, Computer Wins')
        #computer wins
        computer_wins += 1


    elif computer == 2 and play == 1:
        score = 'computer wins'
        print('Paper covers Rock, Computer Wins')
        #computer wins
        computer_wins += 1

    elif computer == 2 and play == 3:
        score = 'player wins'
        print('Scissors cut Paper, Player Wins')
        #player wins
        player_wins += 1


    elif computer == 3 and play == 1:
        score = 'player wins'
        print('Rock smashes Scissors, Player Wins')
        #player wins
        player_wins += 1

    elif computer == 3 and play == 2:
        score = 'computer wins'
        print('Scissors cut Paper, Computer Wins')
        #computer wins
        computer_wins += 1


#call main function
main()
