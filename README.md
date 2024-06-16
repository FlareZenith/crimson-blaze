#include <iostream>
#include <string>

// Define the CrimsonBlaze class
class CrimsonBlaze {
private:
    std::string name;
    int powerLevel;

public:
    // Constructor
    CrimsonBlaze(std::string n, int pl) : name(n), powerLevel(pl) {}

    // Method to get the name
    std::string getName() const {
        return name;
    }

    // Method to set the name
    void setName(std::string n) {
        name = n;
    }

    // Method to get the power level
    int getPowerLevel() const {
        return powerLevel;
    }

    // Method to set the power level
    void setPowerLevel(int pl) {
        powerLevel = pl;
    }

    // Method to display information about the CrimsonBlaze
    void displayInfo() const {
        std::cout << "Name: " << name << ", Power Level: " << powerLevel << std::endl;
    }
};

int main() {
    // Creating an instance of CrimsonBlaze
    CrimsonBlaze blaze("Crimson Blaze", 100);

    // Displaying information using the displayInfo method
    blaze.displayInfo();

    // Changing the power level
    blaze.setPowerLevel(120);

    // Displaying updated information
    blaze.displayInfo();

    return 0;
}
