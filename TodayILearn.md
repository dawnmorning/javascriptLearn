### 자바스크립트란?

웹페이지를 동적으로 만들어주기 위한 언어

### 모던 자바스크립트

자바스크립트 ES6와 그 이후 버전들을 모두 포함한 자바스크립트

### 자바스크립트로 할 수 있는 일

1. 웹개발(react, Vue ..)
2. 서버개발(node.js)
3. 애플리케이션 개발(ReactNative)

### 자바스크립트 동작 방식

자바스크립트 엔진은 자바스크립트 코드를 실행하는 프로그램 또는 인터프리터.
대체적으로 웹 브라우저에서 사용된다.
`codesandbox`활용하기

### 변수란

이름을 가진 저장소

```
let color = "skyblue"
console.log(color) # skyblue
console.log(typeof color) # string
```

### 상수란

```
const color = "skyblue"
color = "yellow" # "color" is read-only
```

### 자료형

원시타입과 비원시타입

#### 원시타입 자료형

프로그램이 실행되는 도중에는 단 하나의 값 만을 가지고 있는 자료형

```
let number = 123
number = "123"  # 원시타입, 한번에 고정되어 있는 값

let array = [1,"2",3]  # 비원시타입, 한번의 여러개의 값

let name
console.log(name)  # undefined
```

'+' 연산을 할 때는 숫자를 문자열로 바꾸어버림.
`parseInt(A) + 15 = A+15`, 명시적 변환

```
let numb = 10
let num2 = "10"

console.log(num1 === num2) # false, 자료형 까지 계산
console.log(num1 == num2) 오직 값 일치만 비교 #true

let num
num = num ?? 20 # undefined 혹은 null이면 20을 할당하라.
```

### 조건문

```
let num = 5
if(num===10){
    console.log("Good")
} else if{
    console.log("Bad")
} else{
    console.log("Normal")
}
```

### switch - case문

```
let fruit = "apple"

switch (fruit) {
    case "banana" :
        console.log("바나나")
        break
    case "orange" :
        console.log("오렌지)
        break
    case "apple":
        console.log("사과)
        break
    default :
        console.log("과일")
}
```

### JavaScript 함수

함수란?

- 같은 동작을 하는 중복된 코드가 여기저기 존재할 때,
- 이들을 하나로 묶어 하나의 명령으로 실행할 수 있게 해주는 기능

```
let num1 = 10
let num2 = 10
let sum = num1 + num2
------------
function add(a,b){
    return a+b
}
add(10,10)
```

### scope

범위, 변수 혹은 함수가 갖게 되는 유효 범위

1. 전역

- 어디서든지 해당 변수에 접근 가능

2. 지역

- 지역을 벗어난 곳에서는 접근 불가능

3. 함수
4. 블록

- 같은 블록에서만(중괄호 블록 내에서만)

```
function print(){
    for (let i = 0; i < 10; i++){
        console.log(`블록스코프: ${i}`)
    }
    console.log(i) # 에러, i is not defined
}
```
