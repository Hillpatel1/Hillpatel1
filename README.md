-#include <iostream>
using namespace std;

void updateValue(int value) {
    value = 55; // This change will not affect the original variable.
    cout << "Inside function: " << value << endl;
}

int main() {
    int a = 20;
    updateValue(a); // a is passed by value
    cout << "In main after function call: " << a << endl; // a remains unchanged
    return 0;
}
