# Composition-code
#include <iostream>
using namespace std;

class Engine {
public:
    Engine() {
        cout << "Engine created!" << endl;
    }
    ~Engine() {
        cout << "Engine destroyed!" << endl;
    }
};

class Car {
private:
    Engine engine;  // Composition
public:
    Car() {
        cout << "Car created!" << endl;
    }
    ~Car() {
        cout << "Car destroyed!" << endl;
    }
};

int main() {
    Car myCar;
    return 0;
}
