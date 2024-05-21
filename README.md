# TBG-Modules
This repository contains the many modules used to store the information for my TBG
This is the main module

# main.py - Kaden Whiteside
# May 17, 2024

# This module connects all the dots by importing all the modules involved in-
# -the project to this file. 

from map_module import create_map, print_map
from inventory_module import print_inventory
from character_module import print_characters
from enemies_module import print_enemies

def main():
    """This function displays all the information about the TBG in
    the python shell."""
    print("Welcomes to my TBG!\n")
    
    # Display the map
    game_map = create_map()
    print("Game Map:")
    print_map(game_map)
    print()
    
    # Display the inventory
    print("Inventory:")
    print_inventory()
    
    # Display characters
    print("Characters:")
    print_characters()
    
    # Display enemies
    print_enemies()

if __name__ == "__main__":
    main()

