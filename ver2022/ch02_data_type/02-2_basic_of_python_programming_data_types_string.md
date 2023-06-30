# 02-1 파이썬 프로그래밍의 기초, 자료형

> "자료형을 알고 있다면 그 언어의 절반을 터득한 것"

## 02-2 문자형
### 문자열 자료형 만드는 4가지 방법

```python
a = "Hello World"
b = 'Python is fun'
c = """Life is to short, You need python"""
d = '''Life is to short, You need python'''
print(a) # Hello world
print(b) # Python is fun
print(c) # Life is to short, You need python
print(d) # Life is to short, You need python
print(type(a)) # <class 'str'>
print(type(b)) # <class 'str'>
print(type(c)) # <class 'str'>
print(type(d)) # <class 'str'>
```

#### 이스케이프 코드란
> "문자열 예제에서 여러 줄의 문장을 처리할 때 백슬래시 (/) 문자와 n을 조합한 '\n' 이스케이프 코드를 사용했다. 이스케이프 코드란 프로그래밍할 때 사용할 수 있도록 미리 정의해 둔 '문자 조합'이다. 주로 출력물을 보기 좋게 정렬하는 용도로 사욯나다."

| 자주 사용되는 코드    | 설명                                     |
|---------------|----------------------------------------|
| **`\n`**      | 문자열 안에서 **줄을 바꿀때** 사용                  |
| **`\t`**      | 문자열 사이에 **탭 간격**을 줄 때 사용               |
| **`\\`**      | 문자 \를 그대로 표현할 때 사용                     |
| **`\'`**      | 작은 따옴표 (**'**)를 그대로 표현할 때 사용           |
| **`\"`**      | 큰 따옴표 (**"**)를 그대로 표현할 때 사용            |

| 자주 사용되는 안는 코드 | 설명                                    |
|---------------|---------------------------------------|
| `\r`          | **캐리지 리턴**(줄 바꿈 문자, 현재 커서를 가장 앞으로 이동) |
| `\f`          | **폼 피드**(줄 바꿈 문자, 현재 커서를 다음 줄로 이동)    |
| `\a`          | **벨 소리**(출력할 때 PC 스피커에서 '삑' 소리가 난다)   |
| `\b`          | 백 스페이스(Back Space)                    |
| `\000`        | `null` 문자                             |

- 위 코드 중에서 활용 빈도가 높은 것은 `\n`, `\t`, `\\`, `\'`, `\"`이다. 나머지는 프로그램에서 잘 사용하지 않는다.

### 문자열 더해서 연결하기 (Concatenation)
```python
a = "Python"
b = " is fun!"

print(a + b) # Python is fun!
```
### 문자열 곱하기

```python
c = "Python"

print(c * 10) # Python 출력 문이 10개 나옴 : PythonPythonPythonPythonPythonPythonPythonPythonPythonPython
```

### 인덱싱(Indexing)
```python
a = "Life is to short, You need Python"

print(a[0]) # L
print(a[1]) # i
print(a[-1]) # n
print(a[-2]) # o
```

- 위 소스 코드에서 변수 a에 저장한 문자열의 각 문자마다 번호를 매겨 보면 다음과 같다

| 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17 | 18 | 19 | 20 | 21 | 22 | 23 | 24 | 25 | 26 | 27 | 28 | 29 | 30 | 31 | 32 | 33 |
|---|---|---|---|---|---|---|---|---|---|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|
| L | i | f | e |   | i | s |   | t | o | o  |    | s  | h  | o  | r  | t  | ,  |    | Y  | o  | u  |    | n  | e  | e  | d  |    | P  | y  | t  | h  | o  | n  |

### 슬라이싱(Slicing)
```python
a = "Life is to short, You need Python"

print(a[0:4]) # Life
```

```python
a = "20010331Rainy"
date = a[:8]
weather = a[8:]

print(date) # 20010331
print(weather) # Rainy
```

```shell
a[  이상  :  미만  :  간격(기본값 1)  ] 
```

$이상 \ \leq x < 미만 \ 간격(default \ 1)$

### 문자열 포매팅(formatting)
```python
a = "I eat %d apples." % 3

print(a) # I eat 3 apples.
```

```python
number = 10
day = "three"
a = "I ate %d apples. so I was sick for %s days." % (number, day)
b = "I ate %s apples. so I was sick for %s days." % (number, day)
c = "abcdefghijklmn {} opqrstuvwxyz".format("안녕")
d = "abc {age} defghijklmn {hoho} opqrstuvwxyz".format(hoho="호호", age=2)

name = "int"
e = f"나의 이름은 {name}입니다"

print(a) # I ate 10 apples. so I was sick for three days.
print(b) # I ate 10 apples. so I was sick for three days.
print(c) # abcdefghijklmn 안녕 opqrstuvwxyz
print(d) # abc 2 defghijklmn 호호 opqrstuvwxyz
print(e) # 나의 이름은 int입니다
```

#### 문자열 포맷 코드

| 코드   | 설명                    |
|------|-----------------------|
| `%s` | 문자열(String)           |
| `%c` | 문자 1개(Character)      |
| `%d` | 정수(Integer)           |
| `%f` | 부동 소수(Floating-point) |
| `%o` | 8진수                   |
| `%x` | 16진수                  |
| `%%` | Literal % (문자 '%' 자체) |

### 소수점 표현
```python
# 간격.소수점 남기는 자리 수
a = "%0.4f" % 3.42134234

print(a) # 3.4213
```

### 문자열 개수 세기(count)
```python
a = "hobby"

print(a.count('b')) # 2
```

### 문자열 위치 알려주기1 (find)
```python
a = "Python is best choice"

print(a.find('b')) # 10
print(a.find('x')) # -1
```

### 문자열 위치 알려주기2 (index)
```python
a = "Life is too short"

print(a.index('t')) # 8
print(a.index(''))  # 0
print(a.index('k')) # ValueError: substring not found
```

### 문자열 삽입(join)
```python
a = ","
b = ",".join(["a", "b", "c"])

print(a.join('abcd')) # a,b,c,d
print(b) # a,b,c
```

### 문자열 소문자를 대문자(upper)와 소문자(lower)로 바꾸기
```python
a = "hi"
b = "HELLO"

print(a.upper()) # HI
print(b.lower()) # hello
```

### 양쪽 공백 지우기(strip)
```python
a = "       hi     "

print(a.strip()) # hi
```

### 문자열 바꾸기(replace)
```python
a = "Life is too short"

print(a.replace("Life", "Your leg")) # Your leg is too short
```

### 문자열 나누기(split)
```python
a = "Life is too short"
b = "a:b:c:d"

print(a.split()) # ['Life', 'is', 'too', 'short'] 
print(b.split(":")) # ['a', 'b', 'c', 'd'] 
```