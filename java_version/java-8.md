# Java 8





### I. String Dedeplication

![https://www.youtube.com/watch?v=OhPGN2Av44E](../.gitbook/assets/screen-shot-2020-12-28-at-5.26.22-pm.png)

* String Dedeplication 추가 \(G1 GC에서만\)
  * chars를 공유한다. string은 계속 새로 생성.
  * char\[\] value는 외부에서 접근하지 못한다. private final
  * [https://stackoverflow.com/questions/32854968/java-8-string-deduplication-vs-string-intern](https://stackoverflow.com/questions/32854968/java-8-string-deduplication-vs-string-intern) 
  * [https://openjdk.java.net/jeps/192](https://openjdk.java.net/jeps/192)
  * 단점\(trade-off\)
    * 약간 CPU를 더 사용 한다.
    * young collectiion을 더 발생 시킨다.



### II. Class unloading with concurrent mark

* 
