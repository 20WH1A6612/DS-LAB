#include <stdio.h>
int binary_rec(int a[], int low, int high, int key);
int main(){
    int a[50], n, i, ans, key, low, high;
    printf("Enter array size");
    scanf("%d", &n);
    printf("Enter array elements");
    for(i = 0; i < n; i++){
        scanf("%d", &a[i]);
    }
    low = 0;
    high = n - 1;
    printf("Enter element to be searched");
    scanf("%d", &key);
    ans = binary_rec(a, low, high, key);
    if(ans == -1)
        printf("Element not found");
    else
        printf("element found at %d position", ans + 1);
    }
    int binary_rec(int a[], int low, int high, int key)
    {
    int mid;
    if(low > high)
        return -1;
    mid = (low + high) / 2;
    if(key == a[mid]){
        return mid;
    }
    else if(key > a[mid]){
        binary_rec(a, mid + 1, high, key);
    }
    else{
        binary_rec(a, low, mid - 1, key);
    }
}
