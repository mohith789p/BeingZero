![image](https://github.com/mohith789p/BeingZero/blob/main/images/Factorial-Recursive.png)

# Program

```java

import java.util.*;

class BeingZero{
    long factorial(int n){
      // Just complete given function
      // Do not write main or input reading or output printing
      // That is already taken care by hidden code
      // Just calculate and return the answer value to caller
        if (n == 1 || n == 0)
            return 1;
        return n * factorial(n-1);

    }
}
```
