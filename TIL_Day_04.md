# TIL Day 03

(이것이 자바다 책 참고하여 정리)
> 2022년 05월 24일 화요일

## Chapter04 조건문과 반복문

### 4.2 조건문(if문, Switch문)
#### 4.2.5 switch문
- 조건 제어문
- 변수가 어떤 값을 갖느냐에 따라 실행문이 선택
- if문보다 코드가 간결

```bash
public class SwitchExample {

	public static void main(String[] args) {
		int num = (int)(Math.random()*6) + 1;
		
		switch(num) {
		case 1:
			System.out.println("1번이 나왔습니다.");
			break;
		case 2:
			System.out.println("2번이 나왔습니다.");
			break;
		case 3:
			System.out.println("3번이 나왔습니다.");
			break;
		case 4:
			System.out.println("4번이 나왔습니다.");
			break;
		case 5:
			System.out.println("5번이 나왔습니다.");
			break;
		case 6:
			System.out.println("6번이 나왔습니다.");
			
		}

	}

}
```

### 4.3 반복문
- 어떤 작업이 반복적으로 실행되도록 하는 것 
- for문, do-while문
- for문과 whiile문은 서로 변환 가능
- for문은 반복 횟수를 알고 있을 때 사용
- while문은 조건에 따라 반복할 때 주로 사용

#### 4.3.1 for문
- for문을 사용하면 코드를 줄일 수 있음
- 개발시간을 줄이고 오류 확률도 줄임
- 초기화식 실행 > 조건식 평가해서 true이면 실행문, false이면 for문 블록 실행X
- 실행문 모두 실행되면 증감식 실행하고 다시 조건식

```
1부터 10까지 출력하는 코드
```

```bash
public class ForPrintFrom1To10Example {

	public static void main(String[] args) {
		for(int i=1; i<=10; i++) {
			System.out.println(i);
		}

	}

}
```
- 초기화식 필요없을 경우 생략 가능
```
1부터 100까지 합을 출력하는 코드
```

```bash
public class ForsumFrom1To100Example {

	public static void main(String[] args) {
		int sum = 0;
		
		for(int i=1; i<=100; i++) {
			sum += i;
			
		}
		
		System.out.println("1~100 합 : " + sum);
	}

}
```
