# REST API

### REST란?

> REpresentational State Transfer의 약자
> <br>
> 자원(문서, 그림, 데이터 등)을 표현하고 상태를 전달하는 것.

<br>
<br>

### REST API 중심 규칙

1. URI는 정보의 자원을 표현해야 한다.
2. 자원에 대한 행위는 HTTP Method(GET, POST, PUT, DELETE 등)로 표현된다.

```
 GET /user/add/1  (BAD)
```

```
 POST /user/1  (GOOD)
```

위 예시와 같이 URI로 정보의 자원을 표현(동사보다는 명사로 표현)하며 행위는 표현하지 않는다.
<br>
자원에 대한 행위는 HTTP Method를 통해 표현한다.

<br>

### REST의 특징

1. **Uniform Interface**
   &nbsp;&nbsp;- 특정 언어나 기술에 종속되지 않고 URI로 표현한 자원에 대한 조작이 가능함.
2. **Stateless**
   &nbsp;&nbsp;- REST 서버에서 상태 정보를 저장하지 않음.
3. **Cacheable**
   &nbsp;&nbsp;- HTTP가 가진 캐싱 기능을 적용할 수 있음.
4. **Self descriptiveness**
   &nbsp;&nbsp;- REST API 메세지만 보고도 쉽게 이해할 수 있는 자체 표현 구조로 되어 있음.
5. **Client-Server**
   &nbsp;&nbsp;- 클라이언트와 서버의 역할이 명확히 구분되어 의존성 줄어듦.
6. **Layer Structure**
   &nbsp;&nbsp;- REST 서버는 다중 계층으로 구성될 수 있으며, 필요에 의해 계층을 추가하여 구조상의 유연성을 가질 수 있음.

<br>

### HTTP 응답 코드

**2xx**: 성공
**3xx**: 리다이렉션 완료
**4xx**: 요청 오류
**5xx**: 서버 오류
