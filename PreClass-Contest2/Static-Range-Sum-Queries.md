![image](https://github.com/mohith789p/BeingZero/blob/main/images/Static-Range-Sum-Queries.png)

# Program

```java
import java.util.*;
import java.io.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        long a[] = new long[n];
        long sum[] = new long[n+1];

        sum[0] = 0;

        for(int i = 0; i < n; i++){
            a[i] = sc.nextLong();

            sum[i+1] = a[i] + sum[i];
        }

        int q = sc.nextInt();
        for(int i = 0; i < q; i++){
            int m = sc.nextInt();
            int l = sc.nextInt();
            long s = sum[l + 1] - sum[m];
            System.out.print(s + " ");

        }

    }
}
```
