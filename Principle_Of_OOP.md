
## 1. 좋은 코드를 판별하는 기준

### 1. 경직성 (Rigidity) 
> The system is hard to change because every time you change one thing, you have to change something else in a never ending succession of changes.

### 2. 부서지기 쉬움 (Fragility)
> A change to one part of the system causes it to break in many other, completely unrelated, parts.

### 3. 부동성 (Immobility)
> It is hard to disentangle the system into components that can be reused in other systems.

### 4. 끈끈함 (Viscosity)
> The development environment is held together with scotch tape and toothpaste. It takes forever to go around the edit, compile, test loop.

### 5. 쓸데없이 복잡함 (Needless Complexity) 
> There are lots of very clever code structures that aren’t acutally necessary right now, but could be very useful one day.

### 6. 필요 없는 반복 (Needless Repetition)
> The code looks like it was written by two programmers named Cut and Paste.

### 7. 불투명성 (Opacity)
> Elucidation of the originator’s intent presents certain difficulties related to convolution of expression.

## 2. 효과적인 객체지향 프로그래밍을 위한 원칙
coupling

### 1. The Single Responsibility Principle(SRP) : 하나의 책임 원칙 
> **A CLASS SHOULD HAVE ONLY ONE REASON TO CHANGE.**
<p>어떤 클래스를 변경해야 하는 이유는 오직 하나 뿐 이어야한다. 다른 말로 풀어쓰면, 1개의 클래스는 1가지 목적을 위해서만 구현되어야 한다는 점이다.
클래서에 포함되어 있는 필드, 매서드는 한 가지 목적으로 구성되어야 하며, 2가지 이상의 용도로 사용되는 클래스는 분리하여 관리되어야 효과적인 객체지향 프로그래밍이 가능하다.</p>

### 2. OCR (The Open - Closed Principle) : 개발 - 폐쇄 원칙
>
<p>소프트웨어 엔티티는 확장에 대해서는 개방되어야 하지만, 변경에 대해서는 페쇄되어야 한다. 클래스를 변경하지 않고도 그 클래스의 환경을 바꿀 수 있어야 한다.</p>

### 3. LSP (Liskov Substitution Principle) : 리스코프 교체 원칙
<p>서브 타입(Sub Type)은 언제나 자신의 기반 타입(Base type)으로 교체할 수 있어야 한다.
클래스 개념을 활용하여 쉽게 말하면, 부모 클래스와 자식 클래스가 있을 때, 부모 클래스를 통해 구현된 코드에서는 자식 클래스를 호출하거나 사용하지 않도록 혹은, 내부에서는 사용이 되더라도 코드상으로는 표출되지 않도록 설계를 해야 한다는 뜻이다.
유도된 클래스의 메서드를 퇴화시키거나 불법으로 만드는 일을 피하라. 기반 클래스의 사용자는 그 기반 클래스에서 유도된 클래스에 대해 아무것도 알 필요가 없어야 한다.</p>

<a href="url"><img src="https://github.com/yeodongbin/img/blob/master/LSP_01.jpg" align="centor" height="300" width="500" ></a>

### 4. DIP (Dependency Inversion Principle) : 의존관계 역전 원칙
<p>A. 고차원 모듈은 저차원 모듈에 의존하면 안 된다. 이 두 모듈 모두 다른 추상화된 것에 의존해야 한다.
B. 추상화된 것은 구체적인 것에 의존하면 안 된다. 구체적인 것이 추상화된 것에 의존해야 한다.
자주 변경하는 컨크리트 클래스 대신 인터페이스나 추상 클래스에 의존하라.</p>

### 5. ISP (Interface Segregation Principle) : 인터페이스 격리 원칙
<p>클라이언트는 자신이 사용하지 않는 메서드에 의존 관계를 맺으면 안된다.
어떤 객체의 사용자에게 그 사용자한테 필요한 매서드만 있는 인터페이스를 제공하라.</p>

## Reference 
<p>[1] UML for Java Programmers, 로버트 C. 마틴 지음</p>
<p>[2] Java 프로그래머를 위한 UML 실전에서는 이것만 쓴다, 로버트 C. 마틴 지음, 이용원, 정지호 옮김</p>
<p>[3] http://www.nextree.co.kr/p6960/ : UML 다이어그램에 대해 자세하게 설명하고 있는 사이트 </p>
<p>[4] https://gmlwjd9405.github.io/2018/07/04/class-diagram.html : UML 다이어그램에 대해 자세하게 설명하고 있는 사이트</p>

