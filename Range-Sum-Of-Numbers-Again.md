![image](https://github.com/mohith789p/BeingZero/blob/main/images/Range-Sum-Of-Numbers-Again.png)

# Program
```java
import java.util.*;
import java.io.*;

class Main {
    public static long RangeSum(long n){
        return n*(n+1) / 2;
    }
    
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        
        for(int i = 0; i < n; i++){
            long a = sc.nextLong();
            long b = sc.nextLong();
            long aSum, bSum;
            if(a > b){
                aSum = RangeSum(a);
                bSum = RangeSum(b - 1);
            }
            else {
                aSum = RangeSum(b);
                bSum = RangeSum(a-1);
            }
            System.out.println(aSum - bSum);
        }
    }
}
```
