# s2_Jake-Laurence-De-Guzman-Paz

         #include <iostream>
      #include <string>
      #include <math.h>
      using namespace std;

      int main()
      {
          string userInput;
          cout << "Enter your full name: " << endl;
          getline(cin, userInput);

          int number;
          int factorial = 1;
          cout << "PLease enter your number: " << endl;
          cin >> number;

          while (cin.fail()) {
              cin.clear();
              cin.ignore(1000, '\n');
              cout << "Please enter a valid number, try again: " << endl;
              cin >> number;
          }

          for (int j = number; j > 0; j--) {
              factorial = j * factorial;

          }
          cout << "----------------------------------------------------------------------------------" << endl;
          cout << "The Factorial is: \n" << factorial << endl;
          cout << "----------------------------------------------------------------------------------" << endl;

          for (int i = 1; i <= 10; i++) {
              cout << number << "x" << i << "=" << number * i << endl;
          }
          cout << "----------------------------------------------------------------------------------" << endl;
          cout << endl;

          int j = 1;
          do
          {
              cout << number << "The power of: " << j << "is: " << pow(number, j) << endl;
              j++;
          } while (j < 11);
      }
