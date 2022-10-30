# Wrapper Class란?
* Java에는 기본 자료형과 참조자료형이 있는데 Wrapper Class란 기본자료형을 참조자료형 처럼 사용하기 위한 Class이다.

# 기본 자료형에 해당하는 Wrapper Class
|기본 자료형 | Wrapper Class|
|-|-|
|byte|Byte|
|short|Short|
|int|Integer|
|long|Long|
|double|Double|
|char|Character|
|float|Float|
|boolean|Boolean|


# 왜쓸까?
1. Wrapper Class는 Object타입이다. Object Type의 경우 Call by Reference이기 때문에 
메소드로 전달된 인수를 수정해야할 경우 Object가 필요하다.
2. Java.util 패키지는 Class객체만 처리하므로 이경우에 사용한다
3. Generic,Java의 Collection 패키지 사용을 위해
4. Multi Thread 환경에서의 동기화(AtomicInteger등 Atomictype)
5. 형변환
6. 기존의 Primitive Type은 Stack 영역에 저장되지만 Reference Type은 Heap에 생성되기에 Garbage Collector를 통한 메모리 관리에 유용하다.