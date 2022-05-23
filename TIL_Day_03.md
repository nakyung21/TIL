# TIL Day 03

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

