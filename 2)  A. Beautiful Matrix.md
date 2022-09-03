
Problem : A. Beautiful Matrix (Codeforces)

Problem link : https://codeforces.com/problemset/problem/263/A

## Solution

```C++
   #include<iostream>
#include<string>
#include<map>
#include<vector>
#include<unordered_map>
using namespace std;

int main()
{
    vector<vector<int>> mat(5,vector<int>(5));
    int a,b;
    for(int i=0;i<5;i++)
    {
        for(int j=0;j<5;j++)
        {
            cin >> mat[i][j];
            if(mat[i][j] == 1)
            {
                a=i;
                b=j;
            }
        }
    }

    cout<<abs(2-a) + abs(2-b)<<endl;
    
    return 0;
}

```
