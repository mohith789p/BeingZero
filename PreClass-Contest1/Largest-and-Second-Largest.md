![image](https://github.com/mohith789p/BeingZero/blob/main/images/Largest-and-Second-Largest.png)

# Program

```java
import java.util.*;
import java.io.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        long arr[] =  new long[n];

        for (int i = 0; i < n ; i++)
            arr[i] = sc.nextLong();


        long large = arr[0];
        long second = arr[0];
        
        for(int i = 1; i < n; i++){
            if(arr[i] > large){
                second = large;
                large = arr[i];
            }
            else if (arr[i] > second && arr[i] != large){
                second = arr[i];
            }
            
        }
        System.out.println(large + " " +  second);
    }
}
```
