![image](https://github.com/mohith789p/BeingZero/blob/main/images/Case-Insensitive-Palindrome.png)

# Program

```java
import java.util.*;
import java.io.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int t = sc.nextInt();
        while(t-- != 0){
            String s = sc.next();
            s = s.toLowerCase();

            int l = 0;
            int r = s.length() -  1;
            boolean f = false;
            while(l < r){
                if(s.charAt(l) != s.charAt(r)){
                    System.out.println("No");
                    f = true;
                    break;
                }
                l++;
                r--;
            }
            if(!f)
                System.out.println("Yes");
        }
    }
}
```
