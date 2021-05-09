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

# **4. 강조**

> **1. 굵게**  
> 단어나 구 전후에 두 개의 별표 또는 밑줄을 추가하여 글자를 굵게 만들어 단어를 강조한다.  
>- 공백은 없도록 한다.  
>- 문자 중간에는 별표는 사용가능 하되, 밑줄은 사용불가능하다.  
```ex)  Love**is**bold (O)	 Love__is__bold (X)```
### 예) 
```
        <Markdown>	                   <HTML>	
I just love **bold text**.	I just love <strong>bold text</strong>.	
```
출력 : I just love **bold text**.

---

```
       <Markdown>	                   <HTML>	
 I just love __bold text__.	I just love <strong>bold text</strong>.	
```
출력 : I just love **bold text**. 

---

```
<Markdown>	         <HTML>
Love**is**bold	Love<strong>is</strong>bold	
```
출력 : Love**is**bold

---

> **2. 기울임꼴**  
> 단어나 구 전후에 하나의 별표 또는 밑줄을 추가하여 글자를 기울여 단어를 강조한다.  
>- 공백은 없도록 한다.  
>- 문자 중간에는 별표는 사용가능 하되, 밑줄은 사용불가능하다.  
```ex)  A*cat*meow (O)	 A_cat_meow (X)```  
### 예)
```
           <Markdown>	                                <Html>
Italicized text is the *cat's meow*.	Italicized text is the <em>cat's meow</em>.  
```
출력 : Italicized text is the *cat's meow*.  

---

```
<Markdown>	                   <Html>
Italicized text is the _cat's meow_.	Italicized text is the <em>cat's meow</em>.	  
```
출력 : Italicized text is the _cat's meow_.  

---

```
<Markdown>	           <Html>
A*cat*meow	      A<em>cat</em>meow  
```  
출력 : A*cat*meow

---

> **3. 굵고 기울임꼴**  
> 단어나 구 전후에 세 개의 별표 또는 밑줄을 추가하여 글자를 굵게 함과 동시에 기울여 단어를 강조한다. 
>- 공백은 없도록 한다.  
>- 문자 중간에는 별표는 사용가능 하되, 밑줄은 사용불가능하다.  
```ex)  This is really***very***important text. (O)	 This is really___very___important text. (X)```  
### 예)
```
           <Markdown>	                               <Html>
This text is ***really important***.	 This text is <strong><em>really important</em></strong>.
```
출력 : This text is ***really important***.  

---

```
           <Markdown>	                               <Html>
This text is ___really important___.	 This text is <strong><em>really important</em></strong>.  
```
출력 : This text is ___really important___.

---

```
           <Markdown>	                               <Html>
This text is __*really important*__.	 This text is <strong><em>really important</em></strong>.  
```  
출력 : This text is __*really important*__.  

---

```
          <Markdown>	                               <Html>
This text is **_really important_**.	 This text is <strong><em>really important</em></strong>.  
```
출력 : This text is **_really important_**.  

---

```
          <Markdown>	                               <Html>
This is really***very***important text.	 This is really<strong><em>very</em></strong>important text.  
```
출력 : This is really***very***important text.  

---