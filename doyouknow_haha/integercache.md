# IntegerCache



```java
Integer a = Integer.valueOf(10);
Integer b = Integer.valueOf(10);

System.out.println(a == b); // true
---
Integer a = Integer.valueOf(256);
Integer b = Integer.valueOf(256);

System.out.println(a == b); // false
```



```java
// Integer.java
public static Integer valueOf(int i) {
    if (i >= IntegerCache.low && i <= IntegerCache.high)
        return IntegerCache.cache[i + (-IntegerCache.low)];
    return new Integer(i);
}
```



jvm 셋팅

```text
 -XX:AutoBoxCacheMax=size.
```

