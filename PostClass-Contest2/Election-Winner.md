![image](https://github.com/mohith789p/BeingZero/blob/main/images/Election-Winner.png)

# Program

```java
import java.util.*;
import java.io.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int t = sc.nextInt();

        while(t-- != 0){
            int mem = sc.nextInt();
            int ele = sc.nextInt();
            int a[] = new int[ele];

            for (int i = 0; i < mem; i++){
                int b = sc.nextInt();
                if(b != -1)
                    a[b - 1] += 1;
            }
            int max = 0;
            for(int i = 0; i<ele; i++){
                if(a[i] > a[max])
                    max = i;
            }
            System.out.println(max + 1);

        }
    }
}
```
