#include <iostream>
using namespace std;
 
// Driver code
int main()
{
    int a = 15, b = 20, max_num, flag = 1;
 
    // Use ternary operator to get the
    // large number
    max_num = (a > b) ? a : b;
 
    while (flag) {
        // if statement checks max_num is completely
        // divisible by n1 and n2.
        if (max_num % a == 0 && max_num % b == 0) {
            cout << "LCM of " << a << " and " << b << " is "
                 << max_num;
            break;
        }
 
        // update by 1 on each iteration
        ++max_num;
    }
    return 0;
}
