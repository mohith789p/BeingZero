![image](https://github.com/mohith789p/BeingZero/blob/main/images/Range-Sum-Judgement.png)

# Program

```java
import java.util.*;
import java.io.*;

class Main {
    public static long RangeSum(long n){
        return n * (n+1) / 2;
    }
    public static void main(String[] args) {
        Scanner read = new Scanner(System.in);
        int n = read.nextInt();
        for(int i = 0; i < n; i++){
            long a = read.nextLong();
            long b = read.nextLong();
            long c = read.nextLong();

            long aSum = RangeSum(a - 1);

            
            long bSum = RangeSum(b);

            long res = bSum - aSum;

            if(res == c){
                System.out.println("NEUTRAL");
            } else if(res > c){
                System.out.println("DECREASE " + (res - c));
            } else {
                System.out.println("INCREASE " + (c - res));
            }
        }
    }
}
```
