![image](https://github.com/mohith789p/BeingZero/blob/main/images/Sum-Of-Digits-Recursive.png)

# Program

```java
import java.util.*;
import java.io.*;

class BeingZero {
    public int solve(int n) {
        // complete the function
        if(n == 0){
            return 0;
        }
        return n % 10 + solve(n/10);
    }
}
```
