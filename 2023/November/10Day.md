# 컴파일과 컴파일러는 무엇인가?
#### 컴파일
```
내가 작성한 코드(원시코드)를 기계어(목적코드)로 바꾸는 과정
```

#### 컴파일러
```
컴파일, 즉 원시코드를 목적코드로 바꾸는 과정을 하는 프로그램
```

> 출처 [ https://opentutorials.org/course/2471/13906 ]


# 컴파일과 컴파일러를 웹으로 해석 해보자.
```
html - 원시코드 (내가 작성한 코드)

이걸 2진수 기계어(목적 코드)로 바꾸는 과정은 컴파일 컴파일 즉, 원시코드를 목적코드로바꾸는 과정을 하는 프로그램

(잘못이해)

HTML은 하이텍스트마크다운랭귀지라 브라우저가 해석해서 출력할뿐 어떠한 컴파일도 없다..

```
> 출처 [ TIL을 시작하게 된 선배님의 조언 / https://watermelonlike.tistory.com/170 ]
[ ERR! ]

```
HTML이 parsing(내일 알아보자) 될 때 script태그를 만나면 parsing이 중지되고 script를 해석, 실행한다고 한다. 이때 이해 해야할게 컴파일러, 인터프리터, JIT 컴파일러를 이해 해야한다.
```
> 출처 [ https://watermelonlike.tistory.com/170 ]

```
브라우저의 내장엔진(V8 - 크롬)에서 스크립트를 읽는다(parsing)
읽은 스크립트를 기계어로 전환. (컴파일)
기계어로 전환된 코드를 실행 (실행)
```
> 출처 [ https://velog.io/@wish/JavaScript는-어떻게-컴파일될까 ]

> 참조 [ https://velog.io/@seungchan__y/자바스크립트는-Compiler-Interpreter-언어다 ]
> 참조 [ https://www.daleseo.com/tsc/ ]