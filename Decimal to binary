#include <iostream>
#include <string>

int main() {
    int choice, numlen, sum, sum2, dnum2;
    float count;
    std::string num1, bin, rem;

    do {
        std::cout << "1 Decimal to Binary:" << std::endl;
        std::cout << "2 Binary to Decimal:" << std::endl;
        std::cout << "3 Quit" << std::endl;
        std::cout << "Enter your choice (1 or 2 or 3): ";
        std::cin >> choice;

        if (!(choice == 1 || choice == 2 || choice == 3))
            std::cout << "Not a valid choice…" << std::endl;
        else {
            if (choice == 3)
                break;
            else {
                if (choice == 1) {
                    // Decimal to Binary
                    std::cout << "Enter a decimal number: ";
                    std::cin >> num1;
                    numlen = num1.length();
                    sum = 0;
                    count = numlen - 1;
                    for (int i = 0; i < numlen; i++) {
                        sum = sum + (num1[i] - 48) * pow(2, count);
                        count = count - 1;
                    }
                    std::cout << "Decimal: " << sum << " converted to Binary: " << sum << std::endl;
                }
                else {
                    // Binary to Decimal
                    std::cout << "Enter a binary number: ";
                    std::cin >> num2;
                    int dnum2 = num2;
                    bin = "";
                    while (num2 > 0) {
                        rem = std::to_string(num2 % 2);
                        bin = rem + bin;
                        num2 = num2 / 2;
                    }
                    std::cout << "Binary: " << dnum2 << " converted to Decimal: " << bin << std::endl;
                }
            }
        }
    } while (true);

    return 0;
}
