# Family Tree Builder - DSA

A C++ program to build and visualize a hierarchical family tree. This application enables users to interactively add family members, define parent-child relationships, and visualize the family tree structure. It robustly handles scenarios where users attempt to add a family member to a specified parent who may or may not exist within the tree.

## Constraints

  * Each individual in the family tree is represented by their name, birthdate, and a list of their children.
  * The family tree begins with a single root individual.
  * The program should support adding and visualizing multiple generations in the family tree.
  * Visualization should use ASCII-based hierarchy representation for clarity.
  * The program should provide user-friendly input validation and error messages for invalid operations

## Solution Description

1. Define the `Individual` class with private attributes for name, birthdate, and a vector of children. Include methods for adding a child, getting the name, birthdate, and children.
2.  Define the `FamilyTree` class with a private attribute for the root individual. Include methods for adding a child, visualizing the family tree, and getting the root.
3. In the `main` function, create an instance of the `FamilyTree` class with a root name and birthdate.
4. Create a vector of `Individual*` called `individuals` and add the root individual to it.
5. Enter a loop to display the main menu and handle user input. Repeat until the user chooses to exit.
6. Inside the loop, display the main menu options:
    * Add Family Member
    * Visualize Family Tree
    * Exit
7. Prompt the user to enter their choice.
8. If the user selects "Add Family Member":
    - Prompt the user for the parent's name, child's name, and child's birthdate.
    - Search for the parent in the `individuals` vector to find the individual to whom the child will be added.
    - Create a new `Individual` for the child and add it as a child of the parent.
    - Add the child to the `individuals` vector.
    - Display a success message.
9. If the user selects "Visualize Family Tree":
    - Call the `visualizeTree` method on the root individual to display the family tree hierarchy.
10. If the user selects "Exit":
    - Display a goodbye message.
    - Break out of the loop to exit the program.
11. If the user enters an invalid choice, display an error message.
12. Repeat the loop until the user chooses to exit.


## Authors

This project is co-owned by: [@AmishiDesai04](https://www.github.com/AmishiDesai04) [@chahelgupta](https://www.github.com/chahelgupta) Arushi Sangle

##

Please don't hesitate to offer suggestions, report any issues you encounter, share your feedback, or engage in any other form of communication! Your input is highly valued and appreciated.
