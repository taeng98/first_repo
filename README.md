# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

---

**순서가 있는 리스트**
1. List 1
2. List 2
    1. List 1
        1. List 1
        
3. List 3

**순서가 없는 리스트**
- List 1
- List 2
    - List 1
        - List 1
- List 3

**순서가 있는 리스트에 순서가 없는 리스트**
1. List 1
2. List 2
    - List 1
        - List 1
        
3. List 3

**순서가 없는 리스트에 순서가 있는 리스트**
- List 1
- List 2
    1. List 1
        1. List 1
- List 3

---

**코드 블럭**
1. 여러줄의 경우
- 코드 블럭은 백틱(물결 따옴표) 3개로 감싸주기
- 윗단 백틱 옆에 언어 명시(가독성 증가)

```python
print("Hello World!)
if x < 10:
    print("Good!")
else:
    print("Bad...")
```

2. 한줄의 경우
- 백틱 하나로 감싸주기

`print("Hello World")`

---

**링크 만들기**
- [텍스트 정보], (소괄호)   
[google](https://google.com)   
[naver](https://naver.com)

**이미지 추가하기**   
1. 웹 상에서의 이미지
- ![이미지대체텍스트](이미지주소)   
![Lorem Picsum Image](https://picsum.photos/200/300)
2. 로컬 환경에서의 이미지
- ![로컬이미지](이미지주소)   
![이미지](.\img.jpg)
![이미지](C:\Users\SSAFY\Codes\Startcamp\0711_Day2\img.jpg)
- 이미지의 크기 고정은 markdown 문법은 지원하지 않음
- HTML을 사용해서 조정할 수는 있음   
<img src =".\img.jpg" width ="100">

---

**텍스트 스타일링**
* 텍스트 **굵게**
* 텍스트 *기울기*
* 텍스트 ~~취소선~~

**인용 문구**
> 대충 멋있는 말 1
>> 대충 멋있는 말 2
>>> 대충 멋있는 말 3
>>>> 대충 멋있는 말 4

---
**표 만들기**
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |

- 정렬하기

| First Header   | Second Header  | Third Header    |
| :------------- | -------------: | :-------------: |
| Content        | Content        | Content         |
| Content        | Content        | Content         |

---

**체크 리스트 작성**
- 지원을 하는 서비스도 있고 안하는 서비스도 있다.
- [ ] a task list item
- [ ] list syntax required
- [ ] normal **formatting**, @mentions, #1234 refs
- [ ] incomplete
- [x] completed

[마크다운 관련 자료 확인](https://support.typora.io/Markdown-Reference/#tables)

---

**마크다운 에디터**
- VS Code - Markdown All in One
- Typora (유료)