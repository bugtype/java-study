---
description: Native method
---

# String intern



```java
    void test(){
        String a = new String("hello");
        String b = new String("hello");
        String c = "hello";
        String d = "hello";
        // native method
        String aa = a.intern();
        String bb = b.intern();
        String cc = c.intern();
        String dd = d.intern();

        System.out.println(a == b); // false
        System.out.println(c == d); // ture
        System.out.println(a == c); // false
        //
        System.out.println(aa == bb); // ture
        System.out.println(cc == dd); // ture
        System.out.println(aa == cc); // ture

    }

```

* [https://www.latera.kr/blog/2019-02-09-java-string-intern/](https://www.latera.kr/blog/2019-02-09-java-string-intern/)

