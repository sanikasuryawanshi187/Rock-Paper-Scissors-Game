import random

def determine_winner(user_choice, computer_choice):
    if user_choice == computer_choice:
        return "It's a tie!"
    elif (user_choice == 'rock' and computer_choice == 'scissors') or \
         (user_choice == 'scissors' and computer_choice == 'paper') or \
         (user_choice == 'paper' and computer_choice == 'rock'):
        return "You win!"
    else:
        return "You lose!"

def play_game():
    choices = ['rock', 'paper', 'scissors']
    user_score = 0
    computer_score = 0

    while True:
        user_choice = input("Enter rock, paper, or scissors (or 'q' to quit): ").lower()
        
        if user_choice == 'q':
            break
        
        if user_choice not in choices:
            print("Invalid choice. Please enter rock, paper, or scissors.")
            continue

        computer_choice = random.choice(choices)
        print(f"You chose {user_choice}. The computer chose {computer_choice}.")

        result = determine_winner(user_choice, computer_choice)
        print(result)

        if result == "You win!":
            user_score += 1
        elif result == "You lose!":
            computer_score += 1
        
        print(f"Score - You: {user_score} | Computer: {computer_score}")

    print("Thanks for playing!")

play_game()
