# CPU Scheduling

### 스케줄링(Scheduling)이란?

`CPU 자원을 프로세스에 어떻게 할당하지?`

프로그램이 실행된 상태인 프로세스는 CPU 자원을 효율적으로 관리하기 위한 abstraction이다. CPU 스케줄러는 프로세스가 생성되면 스케줄링을 통해 CPU 자원의 할당을 결정하며, 이를 통해 컴퓨터 자원을 효율적으로 관리하도록 한다.

<br>

### 선점 스케줄링과 비선점 스케줄링의 비교

**1. 선점 스케줄링(preemptive)**

> 프로세스가 CPU를 할당받아 실행되고 있더라도 운영체제가 CPU를 강제로 빼앗을 수 있는 스케줄링 기법.

<br>

- 장점: 우선순위가 높은 프로세스를 먼저 처리할 수 있는 유연성을 가진다.
- 단점: 우선순위가 높은 프로세스가 생길 때마다 context switching이 자주 일어나게 되어 오버헤드가 크다.

<br>

**2. 비선점 스케줄링(non-preemptive)**

> 프로세스가 CPU를 할당받아 실행되고 있으면 운영체제가 CPU를 강제로 빼앗을 수 없는 스케줄링 기법. 프로세스가 CPU를 할당받고 나면 헤당 프로세스가 완료될 때까지 interrupt 없이 CPU를 사용함.

<br>

- 장점: 필요한 context switching 외에 추가적인 오버헤드가 없으며, 응답 시간의 예측이 쉽다.
- 단점: 중요한 작업이 처리 시간이 길지만 중요하지 않은 작업을 위해 오래 대기하는 상황이 발생할 수 있다.