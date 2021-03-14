# 프로그래밍 시작하기 in Python

## 파이썬 첫 걸음

<br>

### **01 우리가 사용할 도구들**

파이썬 코드를 컴퓨터가 이해할 수 있는 머신 코드로 번역을 해주는게 Python interpreter이다.<br>
Python code > Python interpreter > Computer

PyCharm은 코딩할 때 필요한 여러 프로그램을 하나의 프로그램으로 제공해주는 올인원 솔루션.<br>
이러한 프로그램을 통합 개발 환경, Integerated Development Environment(IDE)라고 한다.

<br>

### **02 파이썬 설치 (Window)**

파이썬 다운로드 공식 사이트 : https://www.python.org/downloads/<br>
파이참 다운로드 공식 사이트 : https://www.jetbrains.com/ko-kr/pycharm/<br>

설치 방법 : 생략

<br>

### **03 파이썬 설치 (Mac)**

파이썬 다운로드 공식 사이트 : https://www.python.org/downloads/<br>
파이참 다운로드 공식 사이트 : https://www.jetbrains.com/ko-kr/pycharm/<br>

설치 방법 : 생략

<br>

### **04 PyCharm 둘러보기**

(생략) 파이썬 기본 사용방법 설명<br>
(생략) 새 파일 생성, 파이썬 파일 생성, 코드 실행 등 간단한 사용 방법 설명

<br>

### **05 print 사용해 보기**

**실습과제**

파이썬에서 *print*라는 것을 사용하면 콘솔에 원하는 내용을 출력할 수 있습니다.<br>
실습창을 보시면 *print(12)*가 이미 작성되어 있는데요.<br>
이건 콘솔에 12를 출력하라는 의미를 가진 코드입니다. 실습창의 실행하기 버튼을 누르면 콘솔에 12가 출력될 것입니다.<br>
이번 과제에서 여러분에게 주어진 업무는 콘솔에 12를 세번 출력하는 것입니다.<br>
12를 출력하는 방법은 수없이 많은데, 몇 가지 예시를 보여드리자면...<br>
```python
print(3 * 4)
print(5 + 7)
print(15 - 3)
```
위에 적혀 있는 세 줄 모두 12를 출력하는 코드입니다.<br>
여러분도 자유롭게 코드를 작성하고, 채점하기 버튼을 클릭해 주세요!<br>

Ans)
```python
print(12)
print(25 // 2)
print(11 + 1)
```

<br>

---

## 프로그래밍 기본 개념

<br>

### **01 코멘트**

코멘트(주석)은 도대체 왜 쓰지?
코딩하다가 메모

코멘트 사용 이유

복잡한 코드 설명
하다가 만 부분 표시
다른 개발자들과 소통

<br>

### **02 자료형 개요**

자료형(Data Type) : 다양한 자료형이 존재한다.

대표적인 자료형 예시
1. 숫자 > 정수(Integer), 소수(Floating Point)
2. 문자(String)
3. 불린(Boolean) : 참(True)과 거짓(False)

2(int)와 2.0(float)와 '2'(str)는 모두 다른 값이다.

<br>

### **03 추상화 개요**

추상화(Abstraction) : 복잡한 내용은 숨기고, 주요 기능에만 신경쓰자!

- 변수(Variable) : 값을 저장하는 것
- 함수(Function) : 명령을 저장하는 것
- 객체(Object)

<br>

### **04 변수**

사용예시)

입력
```Python
burgur_price = 4990

print(burgur_price)
print(burgur_price * 2)
```

결과
```
4990
9980
```

<br>

### **05 칼로리 계산기**

**실습과제**

변수를 배웠으니 한 번 사용해 봅시다. 총 다섯 가지 과자가 있습니다.

- kitkat: 190 칼로리
- oreos: 502 칼로리
- pringles: 292 칼로리
- twix: 135.9 칼로리
- cheetos: 485 칼로리

과자를 다양하게 조합해서 먹었을 때 총 몇 칼로리인지 계산해 보려고 하는데요. 각 과자의 이름을 변수 이름으로 사용하여, 해당 과자의 칼로리를 저장해 주세요.

입력
```Python
kitkat = 190
oreos = 502
pringles = 292
twix = 135.9
cheetos = 485

# 다양한 과자 조합
print(kitkat + oreos * 2)
print(cheetos * 4)
print(pringles + oreos + twix)
print(pringles * 3 + oreos * 2)
```

결과
```
1194
1940
929.9
1880
```

<br>

### **06 함수**

자주 사용되는 함수들은 기본제공된다. 이러한 함수를 내장 함수라고 한다. ex) print함수

내장 함수를 제외한 함수는 직접 만들어주어야 한다.

사용예시)

입력
```Python
def hello():  # 함수 정의
    print("Hello!")
    print("Welcome to Codeit!")

hello()  # 함수 사용
```

결과
```
Hello!
Welcome to Codeit!
```

<br>

### **07 카페 모카 레시피**

**실습과제**

동욱이는 얼마 전 카페 알바를 시작했습니다. 그런데 아직 초짜이다 보니 실수가 잦네요. 실수를 좀 줄이기 위해, 카페 모카의 레시피를 출력하는 함수를 만들어 보려 합니다.<br>
아래의 레시피를 한 줄씩 그대로 출력하도록 함수 cafe_mocha_recipe를 작성하세요.

카페 모카 레시피
1. 준비된 컵에 초코 소스를 넣는다.
2. 에스프레소를 추출하고 잔에 부어 준다.
3. 초코 소스와 커피를 잘 섞어 준다.
4. 거품기로 우유 거품을 내고, 잔에 부어 준다.
5. 생크림을 얹어 준다.

입력
```Python
def cafe_mocha_recipe():
    print("""1. 준비된 컵에 초코 소스를 넣는다.
2. 에스프레소를 추출하고 잔에 부어 준다.
3. 초코 소스와 커피를 잘 섞어 준다.
4. 거품기로 우유 거품을 내고, 잔에 부어 준다.
5. 생크림을 얹어 준다.""")

cafe_mocha_recipe()  # 테스트 코드
```

결과
```Python
1. 준비된 컵에 초코 소스를 넣는다.
2. 에스프레소를 추출하고 잔에 부어 준다.
3. 초코 소스와 커피를 잘 섞어 준다.
4. 거품기로 우유 거품을 내고, 잔에 부어 준다.
5. 생크림을 얹어 준다.
```

<br>

### **08 파라미터**

어떤 파라미터를 넣어주느냐에 따라 함수의 동작이 달라진다.

사용예시)

입력
```Python
def hello(name):  # 함수 정의
    print("Hello!")
    print(name)

hello("Codeit!")
hello("Chris")
```

결과
```
Hello!
Codeit!
Hello!
Chris
```

<br>

### **09 여러 개의 파라미터**

사용예시)

입력
```Python
def print_sum(num1, num2, num3):
    print(num1 + num2 + num3)

print_sum(7, 3, 2)
```

결과
```
12
```

<br>

### **10 세 수의 곱**

**실습과제**

세 수의 곱을 알려주는 프로그램을 만들려고 합니다.

파라미터로 정수 값 세 개를 받고, 세 수의 곱을 출력하는 함수 multiply_three_numbers를 만들어 보세요.

입력
```Python 
def multiply_three_numbers(num1, num2, num3):
    print(num1 * num2 * num3)

# 테스트 코드
multiply_three_numbers(7, 3, 5)
multiply_three_numbers(21, 4, 9)
multiply_three_numbers(-7, 6, 3)
```

결과
```
105
756
-126
```

<br>

### **11 return문**

사용예시)

입력
```Python 
def get_square(x):
    return x * x

print(get_square(3))
y = get_square(4)
print(y)
```

결과
```
9
16
```

<br>

### **12 프로그래밍 기초 퀴즈**

**질문1**

다음 코드를 실행한 출력 결과를 예상해 보세요.

```Python
a = 5
b = 8
c = "5"
d = "8"

print(a + b)
```
1. 10
2. 13
3. 16
4. 58
5. 85

**Ans)** 2

<br>

**질문2**

다음 코드를 실행한 출력 결과를 예상해 보세요.

```Python
a = 5
b = 8
c = "5"
d = "8"

print(c + d)
```
1. 10
2. 13
3. 16
4. 58
5. 85

**Ans)** 4