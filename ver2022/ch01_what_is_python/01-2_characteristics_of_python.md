# 01-2 파이썬 특징

## 파이썬 특징 1
- 파이썬은 인간다운 언어이다

```python
# 4가 [1, 2, 3, 4]안에 있다면 출력해라("xxx")
if 4 in [1, 2, 3, 4]: print ("4가 있습니다")
```

- 파이썬은 문법이 쉬워 빠르게 배울 수 있다
  - 대학교 교양 강의로 파이썬 활용
  - 프로그래밍 유 경험자라면 1주일이면 충분(물론 개인의 차이가 있을 수 있음)
  
## 파이썬 특징 2
- 파이썬은 **무료**이지만 **강력**하다
  - 사용료 걱정없이 언제 어디서든 파이썬을 다운로드하여 사용 가능
  - `Python`과 `C`는 찰떡궁합 (`접착언어`)
    - 상대적으로 쉽지만 느린 `Python` + 복잡하고 어렵지만 빠른 `C`언어 조합 가능
  - `Python` 라이브러리들 중에는 `C`로 만들어진 것도 많다
    - `NumPy` : `C` 라이브러리를 `Python`에서 쓸 수 있도록 래핑
    > '랩핑(wrapping)은 한 언어나 시스템에서 작성된 코드나 라이브러리를 다른 언어나 시스템에서 사용할 수 있도록 적합한 형태로 감싸주는 과정'

### C vs Python
- 컴파일 언어(빠름) vs 인터프리터 언어(느림)

| 컴파일 언어                                                                                                                      |인터프리터 언어|
|-----------------------------------------------------------------------------------------------------------------------------|------------|
| <code>#include <stdio.h><br><br>int main()<br>{<br>&nbsp;&nbsp;printf("Hello")<br>&nbsp;&nbsp;printf("world!")<br>&#9;return 0;<br>}</code> |<code>print('Hello')<br>print('world!')</code>|

- **컴파일 언어란?** : 작성한 코드를 컴퓨터 언어로 바꾸어 0과 1의 기계어로 번역하여 컴퓨터의 실행 프로그램을 작동하게 하는 언어. 즉, 컴퓨터 입장에서는 바로 컴퓨터 언어를 읽을 수 있어서 동작이 빠르다.
- **인터프리터 언어란?** : 작성한 코드를 한줄 씩 인터프리터를 거쳐 컴퓨터에게 전송되는데, 번역하고 읽고의 과정을 거쳐서 상대적으로 느리게 작동하게 된다.

## 파이썬 특징 3
- 파이썬은 간결하다

```python
# simple.py
languages = ['python', 'perl', 'c', 'java']

for lang in languages:
    if lang in ['python', 'perl']:
        print("%6s need interpreter" % lang)
    elif lang in ['c', 'java']:
        print("%6s need compiler" % lang)
    else:
        print("sould not reach here")
```

```
# simple.py 출력
python need interpreter
perl need interpreter
c need compiler
java need compiler
```

- 파이썬은 가장 좋은 방법 1가지만 이용하는 것을 선호
- **실행이 되게 하려면 꼭 줄을 맞추어야 한다**

## 파이썬 특징 4
- 파이썬은 개발 속도가 빠르다
  - "`Life is to short, You need Python.`" (인생은 너무 짧으니 파이썬이 필요하다)