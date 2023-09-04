# Stock-Management-System
This Java code represents a simple Stock Management System that allows users to perform basic operations on a list of stocks. Here's an explanation of the code:

1. **Imports and Class Declaration:**
   - The code begins by importing the necessary Java libraries: `java.util.ArrayList` and `java.util.Scanner`.
   - It defines a class named `StockManagementSystem`, which contains the main method where the program execution starts.

2. **Main Method:**
   - Inside the `main` method, a `Scanner` object named `input` is created to read user input.
   - An `ArrayList` named `stocks` is initialized to store Stock objects. This list will hold information about different stocks.

3. **Menu and User Input:**
   - The program displays a menu with four options: Add stock, Remove stock, View stock, and Exit.
   - It uses a `do-while` loop to repeatedly prompt the user for their choice and execute the corresponding action based on the choice.

4. **Switch Statement:**
   - The program uses a `switch` statement to handle the user's choice:
     - **Case 1 (Add stock):** The user is prompted to enter details for a new stock (name, quantity, and price). A new `Stock` object is created and added to the `stocks` ArrayList.
     - **Case 2 (Remove stock):** The user is prompted to enter the name of the stock and the quantity to remove. It then searches for the stock by name in the `stocks` list and updates the quantity accordingly.
     - **Case 3 (View stock):** It displays the details of all stocks currently stored in the `stocks` ArrayList.
     - **Case 4 (Exit):** The program exits.

5. **Stock Class:**
   - Below the `main` method, a separate class named `Stock` is defined to represent individual stocks.
   - It has private instance variables for the stock's name, quantity, and price.
   - The class provides a constructor to initialize these variables when creating a new stock object.
   - Getter methods (`getName`, `getQuantity`, and `getPrice`) are provided to access the stock's information.
   - The `removeQuantity` method allows for removing a specified quantity from the stock if there is enough quantity available.
   - The `toString` method is overridden to provide a formatted string representation of the stock's details.

6. **Exiting the Program:**
   - The program continues to execute the menu and handle user input until the user chooses to exit (choice 4).
   - After exiting the loop, the `input` Scanner is closed to release resources.

Overall, this code represents a basic stock management system where stocks can be added, removed, and viewed. It demonstrates the use of classes, ArrayLists, user input, and a simple menu-driven interface.
