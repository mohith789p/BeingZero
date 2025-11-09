![image](https://github.com/mohith789p/BeingZero/blob/main/images/Cut-The-Pizza.png)

# Program
```java
import java.util.*;
import java.io.*;

class Main {
    public static void main(String[] args) {
        Scanner read = new Scanner(System.in);
        int n = read.nextInt();

        for(int i = 0; i < n; i++){
            int a = read.nextInt();

            if(a == 1){
                System.out.println("Yes");
            } else if(a % 2 == 0){
                System.out.println("Yes");
            } else {              
                System.out.println("No");
                
            }
        }
    }
}
```
