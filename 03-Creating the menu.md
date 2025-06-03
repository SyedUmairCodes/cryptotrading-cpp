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