# 02-1 파이썬 프로그래밍의 기초, 자료형

> "자료형을 알고 있다면 그 언어의 절반을 터득한 것"

## 자료형 이란?
- 문자의 값을 **숫자**로 인식 할 지, **문자**로 인식 할 지 구분할 수 있게 해주는 것
- 즉, 데이터의 종류에 따른 형태로, 저장되는 값의 종류와 범위에 따라 다르게 표현

### 자료형의 종류
#### 자료에 대한 타입
- `Integer(정수)`, `String(문자열)`, `Boolean(불 - 참/거짓)`

#### 어떤 값을 담는 자료구조
- `Variables(변수)`, `List(리스트)`, `Tuple(튜플)`, `Dictionary(딕셔너리)`

## 02-1 숫자형
- 정수형 (1, 2, -2)
- 실수형 (3.14, -34.23)
- 컴퓨터식 지수 표현 방식 (4.23e10, 4.24e-10) -> $4.23^{10}$, $4.23^{-10}$
- 8진수 (0o37)
- 16진수 (0x7A)

### 사칙연산

```python
a = 3
b = 4

print(a + b)    # 7
print(a - b)    # -1
print(a * b)    # 12
print(a ** b)   # 81 (제곱 - a의 b제곱)
print(a / b)    # 0.75
print(a // b)   # 0 (나눈 몫)
print(a % b)    # 3 (나누고 난 나머지)
```