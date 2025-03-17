# Program-3
    include <iostream>
    include <string>
    include <map>
    using namespace std;

    void countOccurrences(string str) {
        map<char, int> freq;

        for (char c : str) {
            if (isalpha(c)) {  // Consider only alphabets
                freq[tolower(c)]++;
            }
    }

        cout << "Character Frequency Table:\n";
        for (auto pair : freq) {
           cout << pair.first << " -> " << pair.second << endl;
        }
    }

    int main() {
        string input;
        cout << "Enter a string: ";
        getline(cin, input);

        countOccurrences(input);

        return 0;
    }


![image](https://github.com/user-attachments/assets/6c9cdd94-53c1-4513-b9e0-1263c6805c5f)


![image](https://github.com/user-attachments/assets/c305392c-fbe3-40ff-ba6d-16e020241792)



# OUTPUT


![image](https://github.com/user-attachments/assets/5ab467ff-d52c-4cec-affb-5fa62af17784)


