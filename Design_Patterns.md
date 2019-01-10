# Gang of Four

## 1. Creational Design Patterns

### 1.1. Abstract Factory Pattern
- 인터페이스를 이용하여 서로 연관되거나 의존하는 객체를 생성할 수 있다.

### 1.2. Factory Pattern
- 객체를 생성하는 메소드를 Factory Method Pattern 이라고 한다. 즉, 클래스의 인스턴스를 만드는 작업을 서브 클래서에서 맡겨서 진행한다. 생성할 추상 클래스를 상속받은 Sub-class에서 결정한다.

### 1.3. Builder Pattern
- 제품을 여러 단계로 나눠서 만들 수 있도록 제품 생산 단계들을 캡슐화할 때

### 1.4. Prototype Pattern
- 어떤 클래스의 인스턴스를 만드는 것이 자원/시간을 많이 잡아먹거나 복잡한 경우

### 1.5. Singleton Pattern
- 객체를 하나만 생성하여, 생성된 객체를 모든 다른 클래스에서 참조할 수 있도록 하는 디자인 패턴이다.

<pre><code>public class SingletonPatternDemo {
   public static void main(String[] args) {
      SingleObject object = SingleObject.getInstance();
      object.showMessage();
   }
}

public class SingleObject {
   private static SingleObject instance = new SingleObject();
   private SingleObject(){}
   public static SingleObject getInstance(){
      return instance;
   }
   public void showMessage(){
      System.out.println("Hello World!");
   }
}</code></pre>
<pre><code>public class SingletonPatternDemo {
  public static void main(String argv[]) {
    SingleObject.showMessage();
  }
}

final class SingleObject {
  static public void showMessage() {
    System.out.println("Hello World!");
  }
}</code></pre>


## 2. Structural Design Patterns
### 2.1. Adapter Pattern
- 객체를 감싸서 다른 인터페이스를 제공한다.

### 2.2. Composite Pattern
- 클라이언트에서 객체 컬렉션과 개발 객체를 똑같이 다룰 수 있도록 한다.

### 2.3. Proxy Pattern
- 객체를 감싸서 그 객체에 대한 접근을 제어한다.

### 2.4. Flyweight Pattern
- 어떤 클래스의 인스턴스 한 개만가지고 여러 개의 "가상 인스턴스"를 제공하고 싶을 때

### 2.5. Facade Pattern
- 일련의 클래스에 대해서 간단한 인터페이스를 제공한다.

### 2.6. Bridge Pattern
- 구현 뿐만 아니라 추상화된 부분까지 변경시켜야 하는 경우

### 2.7. Decorator Pattern
- 객체를 감싸서 새로운 행동을 제공한다.


## 3. Behavioral Design Patterns

### 3.1. Template Method Pattern
- 알고리즘의 개별 단계를 구현하는 방법을 서브클래스에서 결정한다.

### 3.2. Mediator Pattern
- 서로 관련된 객체 사이의 복잡한 통신과 제어를 한 곳으로 집중시키고자 할 때

### 3.3. Chain of Responsibility Pattern
- 한 요청을 두 개 이상의 객체에서 처리하고 싶을 때

### 3.4. Observer Pattern
- 상태가 변경되면 다른 객체들한테 연락을 돌릴 수 있게 한다.

### 3.5. Strategy Pattern
- 교환 가능한 행동을 캡슐화하고 위임을 통해서 어떤 행동을 사용할지 결정한다.

### 3.6. Command Pattern
- 요청을 객체로 감싼다.

### 3.7. State Pattern
- 알고리즘의 개별 단계를 구현하는 방법을 서브클래스에서 결정한다.

### 3.8. Visitor Pattern
- 다양한 객체에 새로운 기능을 추가해야 하는데 캡슐화가 별로 중요하지 않은 경우

### 3.9. Interpreter Pattern
- 어떤 언어에 대한 인터프리터를 만들 때

### 3.10. Iterator Pattern
- 컬렉션이어떤 식으로 구현되었는지 드러내진 않으면서도 컬렉션 내에 있는 모든 객체에 대해 반복 작업을 처리할 수 있게 한다.

### 3.11. Memento Pattern
- 객체를 이전의 상태로 복구시켜야 하는 경우


## 4. Etc
### 4.1. MVC pattern
- MVC Pattern 이란 소프트웨어를 만들 때 Model, View, Controller 로 구분하여 설계, 개발을 진행하도록하는 디자인 패턴이다.
MVC 가진 장점은 소프트웨어를 분할 해 병렬적으로 개발할 수 있다는 점이다. 소프트웨어 개발은 1인 개발이 불가능할 정도로 크기가 커져가고 있다. 많은 개발자들이 소프트웨어 개발을 위해 협동해야 한다. 대표적인 소프트웨어 부분으로 분리하여 개발을 진행하기 때문에 독립적, 병렬적인 개발이 가능해 진다.

   * Model : 데이터를 다루는 모듈을 모아놓은 파트
   * View : 사용자가 보는 시각적 모듈을 모아놓은 파트
   * Controller : Model, View 파트의 동작을 조정하여 원활한 데이터 이동, 화면 표시 등이 가능하도록 하는 파트
   
### 4.2. 의존성 주입
-
### 4.3. 데이터 접근 객체(DAO)
-
### 4.4. 데이터 전송 객체(DTO)
-

	
</ol>

# Reference 
- https://www.tutorialspoint.com/design_pattern/singleton_pattern.htm
- http://www.java2s.com/Tutorials/Java/Java_Design_Patterns/index.htm
- https://www.tutorialspoint.com/design_pattern/factory_pattern.htm
- http://hyeonstorage.tistory.com/99
- https://www.javacodegeeks.com/2015/09/java-design-patterns.html
