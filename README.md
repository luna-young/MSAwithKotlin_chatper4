# 리액티브 마이크로 서비스 만들기 

Hi! I'm your first Markdown file in **StackEdit**. If you want to learn about StackEdit, you can read me. If you want to play with Markdown, you can edit me. Once you have finished with me, you can create new files by opening the **file explorer** on the left corner of the navigation bar.

## 스프링 웹플럭스의 이해
스프링 웹플럭스는 네티라는 새 애플리케이션 서버를 사용해 리액티브 마이크로서비스를 만들 수 있는, 스프링 프레임워크 5.0에 도입된 새로운 컴포넌트다. 웹플럭스는 리액티브 스트림 패턴 reactive stream pattern을 구현하기 위해 리액터 프레임워크reatore framework를 광범위하게 사용한다. 


## 네티 사용하기 

네티는 원래 넌블로킹 io 작업을 수행할 수 있게 하는 클라이언트-서버 프레임워크를 만들려는 아이디어를 가진 Jboss가 개발했다.  
이런 기능을 위해 리액터reactor 패턴의 메시지 기반 구현을 사용한다.  
네티는 http, ssl/tls 또는 dns같은 주요 알고리즘 및 프로토콜을 지원하지만  http/2, 웹소켓, 구글 프로토콜 버퍼 같은 최신 프로토콜도 지원한다.  

### 
- google protocol buffer? https://developers.google.com/protocol-buffers/docs/javatutorial  
> 프로토토콜 버퍼는 구글에서 개발하고 오픈소스로 공개한, 직렬화 데이타 구조 (Serialized Data Structure)이다. C++,C#, Go, Java, Python, Object C, Javascript, Ruby 등 다양한 언어를 지원하며 특히 직렬화 속도가 빠르고 직렬화된 파일의 크기도 작아서 Apache Avro 파일 포맷과 함께 많이 사용된다.
(직렬화란 데이타를 파일로 저장하거나 또는 네트워크로 전송하기 위하여 바이너리 스트림 형태로 저장하는 행위이다.)
> 프로토콜 버퍼는 하나의 파일에 최대 64M까지 지원할 수 있으며, 재미있는 기능중 하나는 JSON 파일을 프로토콜 버퍼 파일 포맷으로 전환이 가능하고, 반대로 프로토콜 버퍼 파일도 JSON으로 전환이 가능하다.  
> 프로토콜 버퍼를 사용하기 위해서는 저장하기 위한 데이타형을 proto file 이라는 형태로 정의한다. 프로토콜 버퍼는 하나의 프로그래밍 언어가 아니라 여러 프로그래밍 언어를 지원하기 때문에, 특정 언어에 종속성이 없는 형태로 데이타 타입을 정의하게 되는데, 이 파일을 proto file이라고 한다.
> 이렇게 정의된 데이타 타입을 프로그래밍 언어에서 사용하려면, 해당 언어에 맞는 형태의 데이타 클래스로 생성을 해야 하는데, protoc 컴파일러로 proto file을 컴파일하면, 각 언어에 맞는 형태의 데이타 클래스 파일을 생성해준다.
출처: [https://bcho.tistory.com/1182](https://bcho.tistory.com/1182) [조대협의 블로그]
