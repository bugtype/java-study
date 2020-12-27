# G1 GC

* 최소 4GB
* CMS GC의 문제 해결
  * CPU 리소스 차지 문제
  * 메모리 파편화
* Java 9부터 기본으로 G1 GC 사용.

---

* G1GC 라고도 부른다.
* 서버 스타일 컬렉터.
* 큰 메모리를 가진 멀티 프로세서 머신을 위한 컬렉터.
* 높은 확률로 일시 정지 시간에 대한 목표와 높은 처리량을 달성할 것이다.
* `-XX:+UseG1GC` 옵션으로 G1 컬렉터를 켤 수 있다.
* Young Generation Collection 알고리즘: Snapshot-At-The-Beginning\(SATB\)
* Old Generation Collection 알고리즘: Snapshot-At-The-Beginning\(SATB\)



{% embed url="https://perfectacle.github.io/2019/05/11/jvm-gc-advanced/" %}

[https://johngrib.github.io/wiki/jvm-memory/](https://johngrib.github.io/wiki/jvm-memory/)

