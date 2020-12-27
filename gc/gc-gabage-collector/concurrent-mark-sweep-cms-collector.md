---
description: Concurrent Mark Sweep(CMS) Collector
---

# Concurrent Mark Sweep\(CMS\) Collector



* 가비지 컬렉션 일시 정지가 짧은 것을 선호하는 애플리케이션을 위한 컬렉터.
* 이 방식은 프로세서 리소스를 가비지 컬렉션과 공유한다.
* heap 메모리 영역의 크기가 클 때 적합하다.
* GC의 일시 정지 시간을 줄이는 것이 목적이며, 크기가 큰 오래된 객체가 있는 경우에 적합하다.
* `-XX:+UseConcMarkSweepGC` 옵션으로 CMS 컬렉터를 켤 수 있다.
* Young Generation Collection 알고리즘: Parallel
* Old Generation Collection 알고리즘: Concurrent Mark-Sweep

