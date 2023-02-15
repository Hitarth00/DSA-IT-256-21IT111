#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;

void Toh(int n, char scr, char dest, char temp)
{
    if (n==0){
        return;
    }
    Toh(n-1,scr,temp,dest);
    cout<< "Move disk " << n << " from rod " << scr << " to rod " << dest << endl;
    Toh(n-1,temp,dest,scr);
}
int main() {
    int N;
    cin>>N;
    Toh(N,'A','C','B');
    return 0;
}
