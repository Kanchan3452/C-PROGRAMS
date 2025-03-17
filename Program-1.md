# PROGRAM 1

#include <iostream>
#include <cmath>  // For pow()
using namespace std;
double seriesSum(int n) {
    double sum = 0;
    for (int i = 1; i <= n; i++) {
        double term = 1.0 / pow(i, i);
        if (i % 2 == 0) {
            sum -= term;  // Alternate terms are negative
        } else {
            sum += term;
        }
    }
    return sum;
}
int main() {
    int n;
    cout << "Enter the number of terms: ";
    cin >> n;

    cout << "Sum of series: " << seriesSum(n) << endl;
    return 0;
}
![image](https://github.com/user-attachments/assets/a656a0aa-e89c-432c-9801-623a6ad5776f)
# OUTPUT
![image](https://github.com/user-attachments/assets/7551a6b3-5303-433d-b009-1d8f607b98bc)
