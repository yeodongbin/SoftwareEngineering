

## 좋은 코드를 판별하는 기준

### 1. 경직성

### 2. 부서지기 쉬움

### 3. 부동성

### 4. 끈끈함

### 5. 쓸데없이 복잡함

### 6. 필요 없는 반복

### 7. 불투명성



## 효과적인 객체지향 프로그래밍을 위한 원칙

### 1. SRP

### 2. OCR

### 3. LSP (Liskov Substitution Principle) : 리스코프 교체 원칙
서브 타입(Sub Type)은 언제나 자신의 기반 타입(Base type)으로 교체할 수 있어야 한다.
클래스 개념을 활용하여 쉽게 말하면, 부모 클래스와 자식 클래스가 있을 때, 부모 클래스를 통해 구현된 코드에서는 자식 클래스를 호출하거나 사용하지 않도록 
혹은, 내부에서는 사용이 되더라도 코드상으로는 표출되지 않도록 설계를 해야 한다는 뜻이다.

<a href="url"><img src="https://github.com/yeodongbin/img/blob/master/LSP_01.jpg" align="centor" height="300" width="500" ></a>

### 4. DIP (Dependency Inversion Principle) : 의존관계 역전 원칙
A. 고차원 모듈은 저차원 모듈에 의존하면 안 된다. 이 두 모듈 모두 다른 추상화된 것에 의존해야 한다.
B. 추상화된 것은 구체적인 것에 의존하면 안 된다. 구체적인 것이 추상화된 것에 의존해야 한다.

### 5. ISP (Interface Segregation Principle) : 인터페이스 격리 원칙
클라이언트는 자신이 사용하지 않는 메서드에 의존 관계를 맺으면 안된다.





