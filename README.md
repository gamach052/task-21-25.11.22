###  [Task 7 kyu](https://www.codewars.com/kata/5a03b3f6a1c9040084001765/train/java)

Find the total sum of internal angles (in degrees) in an n-sided simple polygon. N will be greater than 2.


### My solution
```Java
public class AngleSum {
    public static int sumOfAngles(int n) {
        return 180*(n-2);
    }
}

```

### Fav solution
```Java
public class AngleSum {
    public static int sumOfAngles(int n) {
        if(n == 3)
            return 180;
        if(n == 4)
            return 360;
        return 180 + sumOfAngles(n-1);
    }
}
```
I like this solution because I like it
