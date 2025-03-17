# Program 13
     #include <iostream>
     #include <stdexcept>
     using namespace std;

     class PrimeException : public exception {
     public:
         const char* what() const throw() {
             return "Number must be greater than 1!";
         }
     };

     // Function to check if a number is prime
     bool isPrime(int num) {
         if (num < 2) {
             throw PrimeException();
         }
    
         for (int i = 2; i * i <= num; i++) {  // Optimization: loop till sqrt(num)
             if (num % i == 0)
                 return false;
         }
    
         return true;
     }

     int main() {
         int num;
         cout << "Enter a number: ";
         cin >> num;

      try {
             if (isPrime(num))
                 cout << num << " is a prime number.\n";
             else
                 cout << num << " is not a prime number.\n";
         } 
         catch (PrimeException& e) {
             cout << "Error: " << e.what() << endl;
         }

         return 0;
     }



![image](https://github.com/user-attachments/assets/3d454c2d-69d1-483e-abab-9422ae59c320)
![image](https://github.com/user-attachments/assets/f3672b8e-7c48-45ff-a1c1-3532beea23f3)
# output
![image](https://github.com/user-attachments/assets/c524aa53-e955-4e5c-805a-224911974603)
![image](https://github.com/user-attachments/assets/4ca2de9c-8340-49b9-bc39-998f1c0d5ad8)







