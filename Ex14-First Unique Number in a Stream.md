# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap
## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm
1. 
2. 
3. 
4.  
5.   

## Program:
```
/*
Program to tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.
Developed by: DIVYA M
RegisterNumber: 212223040043 
*/

import java.util.*;

public class FirstUniqueNumber {
    public static void main(String[] args) {

        int[] stream = {4, 5, 4, 5, 3, 2, 3, 6};

        LinkedHashMap<Integer, Integer> map = new LinkedHashMap<>();
        for (int num : stream) {
            map.put(num, map.getOrDefault(num, 0) + 1);

            System.out.print("Current First Unique Number: ");
            boolean found = false;

            for (Map.Entry<Integer, Integer> entry : map.entrySet()) {
                if (entry.getValue() == 1) {
                    System.out.println(entry.getKey());
                    found = true;
                    break;
                }
            }

            if (!found) {
                System.out.println("No Unique Number");
            }
        }
    }
}


```

## Output:

<img width="490" height="354" alt="image" src="https://github.com/user-attachments/assets/06ac50d8-8b5b-4e78-af96-7d1a89fb123c" />


## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
