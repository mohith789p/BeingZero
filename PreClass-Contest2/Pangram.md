![image](https://github.com/mohith789p/BeingZero/blob/main/images/Pangram.png)

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

            boolean[] alpha = new boolean[26];
            boolean flag = false;

            for(char ch: s.toCharArray()){
                if( ch >= 'a' && ch <= 'z') {
                    int i = ch - 'a';
                    alpha[i] = true;
                }
            }

            for(int i = 0; i < 26; i++){

                if(!alpha[i]){
                    flag = true;
                    break;
                }
            }
            if(!flag)

                System.out.println("YES");
            else
                System.out.println("NO");
        }
    }
}
```
