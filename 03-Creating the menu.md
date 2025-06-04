# Building the Menu

Our primary objective is to create a text-based (console) menu for user interaction. This menu will present the available actions users can take within the simulation.

Menu Options:

- Print Help: Displays instructions and information about how to use the simulator.
- Print Exchange Stats: Shows current market statistics. This is crucial for users to analyze the market before making trades.
- Make an Offer: Allows the user to offer to sell a currency at a specified price.
- Make a Bid: Allows the user to bid to buy a currency at a specified price.
- View My Wallet: Displays the user's current currency holdings (balances).
- Continue / Next Time Step: Advances the simulation to the next time interval.

The simulator will use real-world data, but the user's bids and offers will be incorporated to determine if they could have made a profit.

```C++
#include <iostream>

int main(){
 std::cout << "1 - Open the help menu" << std::endl;
 std::cout << "2 - Show the exchange stats" << std::endl;
 std::cout << "3 - Make an offer on available bids" << std::endl;
 std::cout << "4 - Open the help menu" << std::endl;
 std::cout << "5 - Make a new bid" << std::endl;
 std::cout << "6 - See your wallet" << std::endl;

 return 0;
}
```
## Adding User input

After creating the menu, we now need to  read user input from the console to determine which menu option the user wants to select.

We implement this functionality by storing the user's choice in an integer variable and then print the user's choice back to the console to verify the input was read correctly.

```C++
#include <iostream>

int main(){
 std::cout << "1 - Open the help menu" << std::endl;
 std::cout << "2 - Show the exchange stats" << std::endl;
 std::cout << "3 - Make an offer on available bids" << std::endl;
 std::cout << "4 - Make a new bid" << std::endl;
 std::cout << "5 - See your wallet" << std::endl;
 std::cout << "6 - Continue" << std::endl;
 std::cout << "===============" << std::endl;
 std::cout << "Select options 1-6" << std::endl;

 int userOptions;
 std::cin>> userOptions;
 std::cout<< "You chose: " << userOptions << std::endl;

 return 0;
}
```

Even without doing anything, our code can somewhat work against any wrong or incorrect input that the user can enter.

- Incase of non-numeric input,`std::cin` appears to set the userOption to 0. The input operation fails but the program doesn't crash.

- Floating-point integers are rounded off to the nearest integer value.

- Large Numbers: Inputting a very large number results in the number being rounded and made smaller, fitting within the integer's representable range.
