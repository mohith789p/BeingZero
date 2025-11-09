![image](https://github.com/mohith789p/BeingZero/blob/main/images/Quadrant-Selection.png)

# Program
```java
import java.util.*;
import java.io.*;

class Main {
    public static void main(String[] args) {
       Scanner read = new Scanner(System.in);
        int a = read.nextInt();
        int b = read.nextInt();

        if(a > 0 && b > 0){
            System.out.println(1);
        }
        else if(a < 0 && b > 0){
            System.out.println(2);
        }
        else if(a < 0 && b < 0){
            System.out.println(3);
        }
        else if(a > 0 && b < 0){
            
            System.out.println(4);
        }
    }
}
```
