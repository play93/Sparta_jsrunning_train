# Sparta_jsrunning_train

달리기반 실습 과제입니다.  
1일차에 배운 내용들을 토대로 풀 수 있도록 구성되어 있습니다.

&nbsp;

## 1. 빈칸 채우기 문제

아래 내용에서 빈 칸에 들어갈 항목들을 채워주시고 왜 그렇게 생각했는지
본인의 생각을 간단하게 1줄 정도 같이 적어주세요.

```javascript
1. let uninitialized;
console.log(uninitialized); // 결과값 < undifined >
//값을 지정하지 않아서 

2. < const > apple = "사과";
apple = "바나나"; // TypeError: Assignment to constant variable
/* 
에러 번역 : 상수변수에 할당
이므로 apple은 상수변수
따라서 상수값으로 선언하는 const
*/

3. let lotto = [3, 8, 13, 19, 21, 32];
console.log(lotto[3]); // 결과값 < 19 >
//배열의 순서는 0(오프셋)부터 시작하므로 19

4. 
let mySchedule = ""; //undefined
console.log(mySchedule || false); // < false >
/* || or연산자는 한쪽이 true일때 true를 리턴, 둘다 false일때 false를 리턴하는데 mySchedule의 값이 undefined이므로 false로 리턴*/

console.log(!!mySchedule); // < false >
/*
!!연산자는 값을 boolean(true/false)타입으로 형변환 하는것
mySchedule의 값은 undefined이므로 false 리턴
*/
```


&nbsp;

## 2. 객체 선언해보기
지난 시간에 배웠던 객체(object)를 다시 복습해보며, 아래의 조건을 충족하는 객체를 직접 선언해보세요.

- 자기 자신을 소개하는 객체입니다.
- 이름, 나이, MBTI 세 가지 키와 값이 포함되어 있어야 합니다.
- 콘솔 창에 이름, 나이, MBTI가 나오도록 console.log() 를 찍어보세요.

예시

```javascript
const yeonju = {
    // 조건을 충족하는 코드 작성
    name: "홍연주",
    age: 32,
    mbti: "ISTP"
};

console.log(yeonju['name']);
console.log(yeonju['age']); //''로 안감싸면 undefined가 뜸
console.log(yeonju['mbti']);

```


&nbsp;

## 3. 홀짝 판별기
지난 시간에 배웠던 연산자를 활용하여, 숫자를 입력하면 홀수인지 짝수인지 판별하는 함수를 만들어 보려고 합니다. 다음과 같은 결과값이 나올 수 있도록 코드를 작성해 주세요.

예시

```javascript
function numSet(s) {
    // 코드를 작성해 주세요.

    if(s % 2 === 0){ //2로 나누었을 때 나머지가 0이면 짝수
        return s = "홀수"
    }else{//그렇지 않으면 홀수
        return s = "짝수"
    }

}

console.log(numSet(10)); // 결과값 "짝수";
console.log(numSet(7)); // 결과값 "홀수";
```


&nbsp;

## 4. 계산기 문제
연산자와 함수, 조건문을 토대로 계산기 함수를 하나 만들어 보려고 합니다.
함수에 숫자 , 연산자 , 숫자 세 개의 매개변수를 넣었을 때 해당 연산자를 기준으로 연산을 해서 값을 반환하는 함수를 만들어주세요.

예시
```javascript
function calculate(a, b, c) {
    // 코드를 작성해주세요.
    if(b="+"){
        return a + c;
    }else if(b="-"){
        return a - c;
    }else if(b="*"){
        return a * c;
    }else if(b="/"){
        return a / c;
    }
}

calculate(3, "+", 6); // 결과값 9
calculate(11, "-", 6); // 결과값 5
calculate(6, "*", 3); // 결과값 18
calculate(15, "/", 3); // 결과값 5
```

&nbsp;

## 5. 평균 점수 구하기 [선택 문제]

5번 문제는 필수 문제가 아닌, 4번까지 풀고 여유가 있을 때 풀어보는 선택 문제입니다.


&nbsp;

학교에서 시험을 보았는데 전산 문제로 한 문제의 답이 전부 오답처리가 된 바람에 학생들의 점수를 전부 3점씩 올려주어야 합니다. 

scores에 있는 학생들의 점수를 반복문을 통해 3점씩 올리게 고쳐주시는데 4번 문제를 통해 만든 계산기 함수를 통해 더해주세요.


```javascript
const scores = [36, 62, 72, 55, 86, 95, 92, 48, 81];

function 함수명(scores) {
    // 4번 문제의 계산기 함수를 활용한 코드를 작성해주세요.
}

console.log(scores);
// 기대값: [39, 65, 75, 58, 89, 98, 95, 51, 84]
```
