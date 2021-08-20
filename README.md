
#include <bits/stdc++.h>

using namespace std;
 

float rmsValue(int arr[], int n)
{

    int square = 0;

    float mean = 0.0, root = 0.0;

    for (int i = 0; i < n; i++) {

        square += pow(arr[i], 2);

    }
 


    mean = (square / (float)(n));

    root = sqrt(mean);
 

    return root;
}
 

int main()
{

    int arr[] = { 10, 4, 6, 8 };

    int n = sizeof(arr) / sizeof(arr[0]);
 

    cout << rmsValue(arr, n);
 

    return 0;
}
