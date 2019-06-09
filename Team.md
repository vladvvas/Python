# Python
# The task is to write a code for creating a sport team. It should be possible to add team meebers and their number 
# TODO Create an empty list to maintain the player names
players = []

add_players = input("Would you like to add players to the list? (Yes/No)  ")
while add_players.lower() == "yes":
    name = input("\nPlease, enter the name of the player to add to the team:  ")
    players.append(name)
    add_players = input("Would you like to add another player? (Yes/No)  ")

# print the number of players on the team
print("\nThe number of players is {}".format(len(players)))

# print the player number and the player name
player_number = 1
for player in players:
    print("Player {}: {}".format(player_number, player))
    player_number += 1    


# Select a goalkeeper
keeper = input("Please, select a goalkeeper by selecting a player number. (1-{})".format(len(players)))

# Print the goal keeper's name
keeper = int(keeper)

print("The goalkeeper's name is {}".format(players[keeper - 1]))
