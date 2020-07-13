#include <iostream>
#include <algorithm>
#include <vector>
using namespace std;

class MyClass
{
    /*private variables*/
        vector <int> nums;
        
    public:
        MyClass(vector<int> numbers)
        {
            nums = numbers;
        }
};

void arraysorter(vector<int>&n)
{
    sort(begin(n), end(n));
    for(auto x: n)
    cout<<x<<" ";
}

int main ()
{
    vector <int> nums = {56, 8, 16, 2, 9};
    arraysorter(nums);
    return 0;
}
