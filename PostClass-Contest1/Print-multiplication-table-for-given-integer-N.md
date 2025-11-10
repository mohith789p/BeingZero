![image](https://github.com/mohith789p/BeingZero/blob/main/images/Print-multiplication-table-for-given-integer-N.png)

# Program
```java
import java.util.*;
import java.io.*;

class Main {
    public static void main(String[] args) {
        Scanner read = new Scanner(System.in);
        int n = read.nextInt();
        for (int i = 0; i < n; i++){
            int a = read.nextInt();
            for(int j = 1; j < 11; j++)
                System.out.println(a + " * " + j + " = " + a*j);
            System.out.println();
            
        }
    }
}
```
