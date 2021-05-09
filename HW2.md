# **<야 ! 너도 MARKDOWN 할 수 있어!>**  
- markdown 기본 구문을 익혀보자. 
  
목차

----

1. 제목
2. 단락
3. 줄 바꿈
4. 강조
5. 인용구
6. 목록
7. 코드
8. 수평 규칙
9. 링크
10. 이미지
11. 이스케이프 문자
12. HTML
 
----  

# **1. 제목**  
> 1. 제목을 만들려면 단어나 구 앞에 #을 추가한다. 만들고 싶은 제목의 크기에 따라 #을 한개부터 여섯개까지 달 수 있다.  
>- 주의사항 :  #뒤에 반드시 공백이 있어야함.  
```ex)    # Here's a Heading (O)  /   #Here's a Heading (X)```
>>-  #1개 : 아주 큰 크기의 제목
>>-  #2개 : 조금 큰 크기의 제목  
>>-  #3개 : 보통 크기의 제목  
>>-  #4개 : 조금 작은 크기의 제목  
>>-  #5개 : 아주 작은 크기의 제목  
>>-  #6개 : 굉장히 작은 크기의 제목  
## 예)  

```
    <Markdown>	                      <HTML>	              
# Heading level 1	        <h1>Heading level 1</h1>	
```
```출력 결과 ``` 
# 제목 1

```
    <Markdown>	                      <HTML>
## Heading level 2	        <h2>Heading level 2</h2>	
```
```출력 결과```
## 제목 2

---

```
    <Markdown>	                      <HTML>
### Heading level 3	        <h3>Heading level 3</h3>	
```
```출력 결과```
### 제목 3

---

```
    <Markdown>	                      <HTML>
#### Heading level 4	    <h4>Heading level 4</h4>	
```
```출력 결과```
#### 제목 4

---

```
    <Markdown>	                      <HTML>
##### Heading level 5	    <h5>Heading level 5</h5>	
```
```출력 결과```
##### 제목 5

---

```
    <Markdown>	                      <HTML>
###### Heading level 6	    <h6>Heading level 6</h6>	
```
```출력 결과```
###### 제목 6

---


> 2. 제목을 만드는 또 다른 방법은 텍스트 아래 줄에 ===혹은 ---을 추가하는 것이다.
> 

## 예)
```
  <Markdown>              	<HTML>	
Heading level 1
===============	     <h1>Heading level 1</h1>	
```
```출력 결과 ``` 

Heading level 1
===============	

```
  <Markdown>              	<HTML>	
Heading level 2
---------------	     <h2>Heading level 2</h2>	
```
```출력 결과 ``` 

Heading level 2
---------------	 

---


# **2. 단락**
> 단락을 만들려면 빈 줄을 사용하여 텍스트 줄을 분리한다.  
### 예)
```
<Markdown>
I really like using Markdown.

I think I'll use it to format all of my documents from now on.
__________________________
<HTML>
<p>I really like using Markdown.</p>

<p>I think I'll use it to format all of my documents from now on.</p>	
```
```출력 결과  ```  
I really like using Markdown.

I think I'll use it to format all of my documents from now on.

---


>- 주의사항 : 공백이나 탭으로 문단을 들여쓰지 않아야 한다.
```
ex) 
Don't put tabs or spaces in front of your paragraphs.

Keep lines left-aligned like this. (O)

ex)
    This can result in unexpected formatting problems.

  Don't add tabs or spaces in front of paragraphs. (X)
```
# **3. 줄 바꿈**
>줄을 바꾸려면 두 개 이상의 공백으로 선을 끝내고 엔터를 입력한다.
### 예)
```
<Markdown>
This is the first line.  
And this is the second line.
<HTML>
<p>This is the first line.<br>
And this is the second line.</p>
```
```출력 결과  ```  
This is the first line.  
And this is the second line.

---

>- 주의사항 : 대부분의 경우에 마크 업 언어는 줄 끝에 아무것도 필요하지 않다.  

``` 호환성을 위해 [공백+엔터] 대신 <br> HTML 태그를 이용하기도 한다. ```
```
ex) First line with two spaces after.  
And the next line.

First line with the HTML tag after.<br>
And the next line. (O)

ex) First line with a backslash after.\
And the next line.

First line with nothing after.
And the next line. (X)
```

---