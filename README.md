# DEQUE-DATA-STURCTURE


## DEQUE(덱/데크) 자료구조 ##

> 자바에서의 덱은 인터페이스로 구현되어 있다.
> Deque 인터페이스 이용한 클래스 종류
>> ArrayDeque,LinkedBlockingDeque,ConcurrentLinkedDeque,LinkedList 등의 클래스로 구현된다.

### DEQUE 메소드 정의 및 역할 ###
#### Deque 입력 메소드 ####
![image](https://user-images.githubusercontent.com/67618667/145753064-d7e50d5d-d10c-4e6c-ba7f-a60e32a21070.png)

1)addFirst()
: 덱의 앞쪽에 엘리먼트를 삽입한다. 용량 제한이 있는 덱의 경우, 용량을 초과하면 예외(Exception) 을 발생한다.

2)offerFirst()
: 덱의 앞쪽에 엘리멘트를 삽입한다. 정상적으로 삽인된 경우 true를 반환한다. 용량 초과가 될 시 false를 반환한다.

3)addLast()
: 덱의 마지막 쪽에 엘리멘트를 삽입한다. 용량 제한이 있는 덱의 경우 , 용량 초과시 예외가 발생한다.

add()는 addLast() 와 동일함

4)offerLast()
:덱의 마지막 쪽에 엘리먼트를 삽입한다. 정상적으로 엘리먼트가 삽입된 경우 true 반환되고 용량 제한에 걸리는 경우 false 를 반환

#### Deque 출력 메소드 ####
![image](https://user-images.githubusercontent.com/67618667/145753471-ded2dcc8-fb59-4300-8120-43330814ec6f.png)

1)removeFirst()
: 덱의 앞쪽에서 엘리먼트 하나를 뽑아서 제거한 다음 해당 엘리먼트를 리턴한다. 덱이 비어있으면 예외가 발생한다.

2)pollFirst()
: 덱의 앞쪽에서 엘리먼트 하나를 뽑아서 제거한 다음 해당 엘리먼트를 리턴한다. 덱이 비어있으면 null을 리턴한다.

3)removeLast()
: 덱의 마지막 쪽에서 엘리먼트 하나를 뽑아서 제거한 다음 해당 엘리먼트를 리턴한다. 덱이 비어있으면 예외가 발생한다.

4)pollLast()
:덱의 마지막 쪽에서 엘리먼트하나를 뽑아서 제거한 다음 해당 엘리먼트를 리턴한다. 덱이 비어있으면 null을 리턴한다.

5)remove()
:removeFirst() 와 동일

6)poll()
: pollFirst() 와 동일

#### Deque get 메소드 ####
![image](https://user-images.githubusercontent.com/67618667/145754318-4736b1fc-c16c-4374-8765-e12124166aaf.png)

1)getFirst()
:덱의 앞쪽 엘리먼트 하나를 제거하지 않은채 리턴한다. 덱이 비어있으면 예외가 발생한다.

2)peekFirst()
:덱의 앞쪽 엘리먼트 하나를 제거하지 않은채 리턴한다. 덱이 비어있으면 null을 리턴한다.

3)getLast()
:덱의 마지막쪽 엘리먼트 하나를 제거하지 않은채 리턴한다. 덱이 비어있으면 예외가 발생한다.

4)peekLast()
:덱의 마지막 엘리먼트 하나를 제거하지 않은 채 리턴한다. 덱이 비어있으면 null을 리턴한다.

5)peek() == peekFirst()와 동일

6)removeFirstOccurrence(Object o)
: 덱의 앞쪽에서부터 탐색하여 입력한 Object와 동일한 첫 엘리먼트를 제거한다. Object o 와 같은 엘리먼트가 없으면 덱에 변경이 발생하지 않는다.

7)removeLastOccurrence(Object o)
: 덱의 뒤쪽에서부터 탐색하여 입력한 Object와 동일한 첫 엘리먼트를 제거한다. Object o 와 같은 엘리먼트가 없으면 덱에 변경이 발생하지 않는다.

8)element()
:removeFirst() 와 동일

9)addAll(Collection <? extends E c)
: 입력 받은 Collection의 모든 데이터를 덱의 뒤쪾에 삽입한다.

10)push()
: addFirst() 와 동일, 덱을 스택으로 사용할 때 쓰임

11)pop()
: removeFirst()와 동일, 덱을 스택으로 사용할 때 쓰임

12)remove(Object o)
: removeFirstOccurrence(Object o) 와 동일

13)contain(Object o)
: 덱에 Object o 와 동일한 엘리먼트가 포함되어 있는지 확인

14)size()
:덱의 크기

15)iterator()
:덱의 앞쪽부터 순차적으로 실행되는 이터레이터(iterator)를 얻어옴

16)descendingterator()
:덱의 뒤쪽부터 순차적으로 실행되는 이터레이터(iterlator)를 얻어옴
