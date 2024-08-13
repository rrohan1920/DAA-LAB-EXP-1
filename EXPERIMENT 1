#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;

void bubbleSort(int arr[], int n)
{
    int i, j;
    bool swapped;
    for (i = 0; i < n - 1; i++) {
        swapped = false;
        for (j = 0; j < n - i - 1; j++) {
            if (arr[j] > arr[j + 1]) {
                swap(arr[j], arr[j + 1]);
                swapped = true;
            }
        }

        if (swapped == false)
            break;
    }
}

void selectionSort(int arr[], int n)
{
    int i, j, min_idx;

    for (i = 0; i < n - 1; i++) {
        min_idx = i;
        for (j = i + 1; j < n; j++) {
            if (arr[j] < arr[min_idx])
                min_idx = j;
        }
        if (min_idx != i)
            swap(arr[min_idx], arr[i]);
    }

}
void printArray(int arr[], int size)
{
    int i;
    for (i = 0; i < size; i++)
        cout << " " << arr[i];
}

int main() {
    
    int startTime = time(NULL);
    int N;
    
    cout<<"Enter the size of array: ";
    
    cin>>N;
    int arr[N];
    for(int i=0; i<N; i++){
        arr[i] = rand()%N;
    }
 
    bubbleSort(arr, N);
    cout << "Sorted array: \n";
  
    printArray(arr, N);
    int endTime = time(NULL);
    cout<<endl<<"Time Taken: "<<endTime - startTime<<endl;
    
    int startTime1 = time(NULL);
    selectionSort(arr, N);
    cout << "Sorted array: \n";
  
    printArray(arr, N);
    int endTime1 = time(NULL);
    cout<<endl<<"Time Taken: "<<endTime1 - startTime1<<endl;
    return 0;
}
