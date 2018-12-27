# Gang of Four

## 1. Creational Design Patterns

### 1. Abstract Factory Pattern

### 2. Builder Pattern

### 3. Factory Pattern

#### 3-1 Abstract Factory Pattern
- 인터페이스를 이용하여 서로 연관되거나 의존하는 객체를 생성할 수 있다.

#### 3-2 Factory Method Pattern
- 객체를 생성하는 메소드를 Factory Method Pattern 이라고 한다. 즉, 클래스의 인스턴스를 만드는 작업을 서브 클래서에서 맡겨서 진행한다.

### 4. Prototype Pattern
### 5. Singleton Pattern
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
### 1. Adapter Pattern
### 2. Composite Pattern
### 3. Proxy Pattern
### 4. Flyweight Pattern
### 5. Facade Pattern
### 6. Bridge Pattern
### 7. Decorator Pattern

## 3. Behavioral Design Patterns
### 1. Template Method Pattern
### 2. Mediator Pattern
### 3. Chain of Responsibility Pattern
### 4. Observer Pattern
### 5. Strategy Pattern
### 6. Command Pattern
### 7. State Pattern
### 8. Visitor Pattern
### 9. Interpreter Pattern
### 10. Iterator Pattern
### 11. Memento Pattern
### 12. MVC pattern

# Reference 
- https://www.tutorialspoint.com/design_pattern/singleton_pattern.htm
- http://www.java2s.com/Tutorials/Java/Java_Design_Patterns/index.htm
- https://www.tutorialspoint.com/design_pattern/factory_pattern.htm
- http://www.java2s.com/Tutorials/Java/Java_Design_Patterns/0010__Java_Factory_Pattern.htm
