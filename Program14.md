# Program 14
     #include <fstream>
     #include <iostream>
     using namespace std;

     void removeWhitespace(string inputFile, string outputFile) {
         ifstream in(inputFile);
         ofstream out(outputFile);

         if (!in || !out) {
             cout << "Error opening files!" << endl;
             return;
         }

         char ch;
         while (in.get(ch)) {
             if (!isspace(ch))
                 out.put(ch);
         }

         cout << "File copied successfully without whitespaces.\n";
         in.close();
         out.close();
     }

     int main() {
         string inputFile = "input.txt";
         string outputFile = "output.txt";

         removeWhitespace(inputFile, outputFile);

         return 0;
     }




![image](https://github.com/user-attachments/assets/4d0cff03-6b48-4945-9ea9-ec93bddac6fe)
![image](https://github.com/user-attachments/assets/c09f04ef-8376-47da-8bb8-aa81cf2c1dfa)



# output
![image](https://github.com/user-attachments/assets/952bf8d4-a992-4aad-9cda-336c6fd48c44)


