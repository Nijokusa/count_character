/* A program to counts the number of characters input
   by the user on one line. The line is terminated by
   a return.  The return is not counted as a character. */

#include <iostream>

using namespace std;

int main()
{
  char ch;                  // store input character
  int num_chars = 0;      // Counts number of characters
  cout << "Enter any number of characters terminated by return."
       << endl << endl;

  ch = cin.get();  // Obtain the first character

  while (ch != '\n')
  {
    ++num_chars;
    ch = cin.get();
  }

  cout << endl;
  cout << "You entered " << num_chars << " characters." << endl;

  return 0;
}
