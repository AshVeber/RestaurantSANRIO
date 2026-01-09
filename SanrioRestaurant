#include <iostream>
#include <vector>
#include <string>
#include <algorithm>

int main() {

    using namespace std;

    string input;
    string a;

    double total = 0;
    vector<string> order = {};
    vector<string> eats = {"Bubble Tea", "Strawberry Mochi", "Peanut toast", "Blueberry pancakes"};
    vector<double> prices = {10.99, 4.55, 9.00, 11.02};

    cout << "     ----------------\n\tRestaurant \n\t  SANRIO \n     ----------------" << "\n";
    cout << "Hello, dear customer! Welcome to Sanrio!\nChoose ur waiter:\n1. My Melody\n2. Cinnamoroll\n3. Hello Kitty\n4. Kuromi\n>> ";
    getline(cin, input);
    if(input.find("My Melody") != string::npos || input.find("1") != string::npos || input.find("1.") != string::npos) {
        cout << "Hi, sweetie! I'm Melody! Here's your menu!\n";
    }else
    if(input.find("Cinnamoroll") != string::npos || input.find("2") != string::npos || input.find("2.") != string::npos) {
        cout << "Hello! I'm Cinnamoroll and I'll be your waiter today!\n It's your menu!\n";
    }else
    if(input.find("Hello Kitty") != string::npos || input.find("3") != string::npos || input.find("3.") != string::npos) {
        cout << "Oh, hi! My name's Hello Kitty. I am your waiter today!\nYour menu!\n";
    }else
    if(input.find("Kuromi") != string::npos || input.find("4") != string::npos || input.find("4.") != string::npos) {
        cout << "Hey! My name is Kuromi!\n Here's your menu!\n";
    }
    cout << "********************\n        MENU\n********************\n";
    for(size_t i = 0; i < eats.size(); ++i) {
        cout << eats[i] << " ---- $" << prices[i] << "\n";
    }
    cout << "What can I get for you today?\n";
    cout << ">> ";
    getline(cin, input);
    if(input.find("Bubble Tea") != string::npos) {
        order.push_back("Bubble Tea");
        total += prices[0];
    }else
    if(input.find("Strawberry Mochi") != string::npos) {
        order.push_back("Strawberry Mochi");
        total += prices[1];
    }else
    if(input.find("Peanut toast") != string::npos) {
        order.push_back("Peanut toast");
        total += prices[2];
    }else
    if(input.find("Blueberry pancakes") != string::npos) {
        order.push_back("Blueberry pancakes");
        total += prices[3];
    }
    if(order.empty()) {
        cout << "You did not order anything!" << "\n>> ";
        getline(cin, input);
    }else {
        for(string orders : order) {
            cout << "Here's your order: " << orders << "\n";
            cout << "Your total price is: $" << total << "\n";
            cout << "Your order will be ready for 15 minutes!\n";
            break;
        }
    }

    return 0;
}
