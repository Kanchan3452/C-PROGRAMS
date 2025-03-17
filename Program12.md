# Program 12
     #include <iostream>
     using namespace std;

     class Student {
     public:
         int rollNo;
         string name;
         string className;
         int year;
         float totalMarks;

         void input() {
             cout << "Enter Roll No, Name, Class, Year, and Total Marks: ";
             cin >> rollNo >> name >> className >> year >> totalMarks;
         }

         void display() {
             cout << "Roll No: " << rollNo << "  Name: " << name << endl;
             cout << "Class: " << className << "  Year: " << year << endl;
             cout << "Total Marks: " << totalMarks << endl;
         }
     };

     int main() {
         Student students[5];

         // Taking input for 5 students
         for (int i = 0; i < 5; i++) {
             cout << "Enter details for Student " << i + 1 << ":\n";
             students[i].input();
         }

        cout << "\nStudent Details:\n";
         for (int i = 0; i < 5; i++) {
             students[i].display();
         }

         return 0;
     }



![image](https://github.com/user-attachments/assets/90b8657e-1482-4d27-93b1-592fa4486228)
![image](https://github.com/user-attachments/assets/bbb180cd-7a21-4a9e-9fb0-9c23ecd1ed8d)
# outout
![image](https://github.com/user-attachments/assets/c4b06aed-414d-4c56-b3cc-7abdb7bc03ff)
![image](https://github.com/user-attachments/assets/540162a0-2186-4239-a162-f712c6d494e8)
