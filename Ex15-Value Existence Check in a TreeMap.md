# Ex15 Value Existence Check in a TreeMap
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm
1. 
2. 
3. 
4.  
5.   

## Program:
```
/*
Program to checks whether a given value exists in a TreeMap.
Developed by: DIVYA M
RegisterNumber:  212223040043
*/

import java.util.*;

public class TreeMapValueCheck {
    public static void main(String[] args) {

        // Creating a TreeMap
        TreeMap<Integer, String> map = new TreeMap<Integer, String>();
        map.put(1, "Apple");
        map.put(2, "Banana");
        map.put(3, "Cherry");
        map.put(4, "Mango");

        // Display TreeMap
        System.out.println("TreeMap Elements: " + map);

        // Value to search
        String searchValue = "Mango";

        // Check value existence
        if (map.containsValue(searchValue)) {
            System.out.println("Value '" + searchValue + "' exists in the TreeMap.");
        } else {
            System.out.println("Value '" + searchValue + "' does NOT exist in the TreeMap.");
        }
    }
}

```

## Output:

<img width="490" height="354" alt="image" src="https://github.com/user-attachments/assets/5b854451-6a10-42b3-8d88-c5f9eaf5317a" />


## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
