# SOLID

### SOLID (객체지향 설계 원칙)

**1. Single Responsibility Principle: 단일 책임의 원칙**
<br>

> 하나의 클래스는 하나의 목적을 위해서 생성.
> <br>
> 응집도는 높게, 결합도는 낮게

<br>

**2. Open Close Principle: 개방 폐쇄 원칙**
<br>

> 소프트웨어의 구성요소는 확장에는 열려있고, 변경에는 닫혀 있어야 함.

<br>

**3. Liskov Substitution: 리스코프 치환의 원칙**
<br>

> 상속받은 하위 클래스는 상위 클래스로 교체될 수 있어야 함.
> <br>
> 오버라이딩으로 상위 클래스의 메소드를 재정의할 때 확장만 되어야 함.

<br>

**4. Interface Segregation Principle: 인터페이스 분리의 원칙**
<br>

> 한 클래스는 자신이 사용하지 않는 인터페이스는 구현하지 말아야 함.

<br>

**5. Dependency Inversion Principle: 의존성 역전의 원칙**
<br>

> 추상을 매개로 메세지를 주고받음으로써 관계를 최대한 느슨하게 함.
> <br>
> 변화가 적은 쪽과 의존 관계를 맺어야 함. (추상 클래스 또는 인터페이스를 참고하도록)
