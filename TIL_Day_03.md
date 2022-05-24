# TIL Day 03

(이것이 자바다 책 참고하여 정리)
> 2022년 05월 23일 월요일

## Chapter04 조건문과 반복문

### 4.1 코드 실행 흐름 제어
- 제어문의 종류
- - 조건문 
- - - if문, Switch문 
- -  반복문
- - - for문, while문, do-while문

### 4.2 조건문(if문, Switch문)
#### 4.2.1 if문
- 조건식의 결과에 따라 블록 실행 여부 결정
- 조건식이 true이면 블록 실행, false이면 블록 실행X
- 중괄호 {} 블록은 여러 실행문을 묶을 때 이용

#### 4.2.2 if-else문
- if문의 조건식이 true이면 if문의 블록 실행, 조건식이 false이면 else 블록이 실행
- 조건식의 결과에 따라 두 개 중 한나의 블록만 실행하고 전체 if문을 벗어남

```
if ~ else 문 예제 
score : 85
90 이상이면
“점수가 90보다 큽니다” “ 등급은 A입니다” 출력
90 보다 작으면
“점수가 90보다 작습니다” “ 등급은 B입니다” 출력
```

```bash
public class IfElse {

	public static void main(String[] args) {
		
		int score = 85;

		if (score >= 90) {
			System.out.println("점수가 90보다 큽니다");
			System.out.println("등급은 A 입니다");
		} else {
			System.out.println("점수가 90보다 작습니다.");
			System.out.println("등급은 B 입니다.");
		}

	}

}
```
#### 4.2.3 if-else if-else문
- 조건문이 여러개인 if문
- 처음 if문의 조건식이 false일 경우 다른 조건식의 결과에 따라 실행 블록 선택 가능 > if 블록 끝에 else if를 붙이면 됨
- else if의 제한X
- 여러 조건식 중 true가 되는 블록만 실행하고 전체 if문을 벗어남
- else if 블록의 마지막에는 else 블록을 추가 가능한데, 모든 조건식이 false인 경우 else 블록을 실행하고 if문을 벗어남

```bash
public class IfElseIfElseEx {

	public static void main(String[] args) {
		
		int score = 75;
		
		if(score>=90) {
			System.out.println("점수가 100~90 입니다");
			System.out.println("등급은 A 입니다");
		} else if(score>=80) {
			System.out.println("점수가 80~89 입니다");
			System.out.println("등급은 B 입니다");
		} else if(score>=70) {
			System.out.println("점수가 70~79 입니다");
			System.out.println("등급은 C 입니다");
		} else {
			System.out.println("점수가 70 미만 입니다");
			System.out.println("등급은 D 입니다");
					
		}
		
	}

}
```

```
- 주사위 번호 뽑기 연삭식
int num = (int) (Math.random() * 6) + 1;
```

```bash
public class IfDiceExample {

	public static void main(String[] args) {
		
		int num = (int)(Math.random()*6)+1; // 주사위 번호 하나 뽑기
		
		if(num==1) {
			System.out.println("1번이 나왔습니다.");
		} else if(num==2) {
			System.out.println("2번이 나왔습니다.");
		} else if(num==3) {
			System.out.println("3번이 나왔습니다.");
		} else if(num==4) {
			System.out.println("4번이 나왔습니다.");
		} else if(num==5) {
			System.out.println("5번이 나왔습니다.");
		} else {
			System.out.println("6번이 나왔습니다.");
			
		}
	}

}
```
