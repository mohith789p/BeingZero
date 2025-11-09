![image](https://github.com/mohith789p/BeingZero/blob/main/images/Even-Division.png)

# Program
```java
import java.util.*;
import java.io.*;

class Main {
    public static void main(String[] args) {
        Scanner read = new Scanner(System.in);
        int n = read.nextInt();
        for(int i = 0; i < n; i++){
            long a = read.nextLong();
            if(a == 2){
                System.out.println("NO");
            }
            else {
            System.out.println( a % 2 == 0 ? "YES" : "NO");
            }
        }
        read.close();
    }
}
```
