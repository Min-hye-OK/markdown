# markdown
마크다운 연습하기
***
## markdown 이란?
```
markdown은 일반 텍스터 문서의 양식을 편집하는 문법이다.
일반 텍스트 편집기로 문서 양식을 편집할 때 쓰임.
마크다운을 이용해 작성된 문서는 쉽게 HTML 등 다른 문서 형태로 변환이 가능함.
```
## markdown Header
```
markdown header는   
# h1  
## h2  
### h3  
#### h4
##### h5
###### h6
위의  6가지 hashtag를 통해 이루어지며 
hashtag 개수에 따라 글자의 크기가 달라집니다.
```

#h1  
##h2  
###h3  
####h4  
#####h5  
######h6  

##줄바꿈
markdown에서 줄바꿈을 하기 위해서는 enter키 입력전 입력 문장의 끝에 공백을 두 개 넣어야 한다.
```
첫 번째 문장 두 번째 문장 세 번째 문장
```
#### *공백을 두번 넣지 않은 경우(공백을 한 번을 넣더라도 동일하다.)
첫번째 문장 
두번째 문장 
세번째 문장 

#### * enter키 입력 전 문장의 끝에 공백을 두 개 넣은 경우
첫번째 문장  
두번째 문장  
세번째 문장

## 문자 강조
 

#### 이탤릭체

기울어진 글씨를 사용하기 위해서는
```
*입력하고자 하는 문장*
_입력하고자 하는 문장_
```
형태로 작성해야 합니다.

*입력하고자 하는 문장*  
_입력하고자 하는 문장_

---
####볼드체
굵은 글씨를 사용하기 위해서는
```
**문장**
__문장__
```
형태로 작성해야 합니다.

**문장**  
__문장__  

문장 내부에서 이탤릭체와 볼드체 모두 혼용하여 사용이 가능합니다.

***이탤릭체+볼드체***  
___이탤릭체+볼드체___  
__볼드체 *이탤릭체+볼드체*__  
_이탤릭체**이탤릭체+볼드체**_

####취소선 넣기
```
~~취소선~~
```  
~~취소선~~  

##링크 이용

```
[링크에 사용할 이름](URL)
ex) [마크다운설명서](https://github.com/Min-hye-OK/markdown.git)

https://github.com/Min-hye-OK/markdown.git
```
[마크다운설명서](https://github.com/Min-hye-OK/markdown.git)

https://github.com/Min-hye-OK/markdown.git

##이미지 넣기
```
![이미지 이름](이미지파일경로.jpg)
![이미지 이름](이미지파일URL)
```
![고라니](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Hydropotes_inermis_male.JPG/1200px-Hydropotes_inermis_male.JPG)
  
## 코드 블럭 사용
github gist에 바로 작성하는 경우 바로 변환되어 보이기 때문에 코드를 보여줄 수 없으므로   
이를 해결하기 위한 문법

* Space Bar 4번 사용  


    for(i=0; ~~~~~~)
    
* `키 3번 사용
```
    ```
    for(i=0;~~~~)
    ```
```
* ~키 3번 사용
~~~

    ~~~
    for(i=0; ~~~~~)
    ~~~
~~~

##테이블

표를 만들어줌

* 칸을 구분 하기 위해서는 |를 이용한다.
* 머리 부분을 -를 이용해 구분해주고 다리 부분을 만들어줘서 테이블을 생성한다.
 
 머리1|머리2|머리3|뚝배기
 ---|---|---|---
다리1|다리2|다리3|다리4|     

##github 사용
1. git clone URL
```
git clone https://~~~
```
git hub repo의 주소를 복사한다.

2. cd ~
```
cd markdown
```
cd명령어는 change directory명령으로 작업하고자 하는 directory로 이동하는 명령어이다.

3. git add " ~ "

stage 영역은 commit할 파일들을 올려놓는 가상 영역인데,
이 stage영역을 이용하여 작업내용 중 특정 파일들만 선별하여 commit에 반영할 수 있음
  
  위의 명령어는 변경된 특정 파일을 stage 영역에 올림

4. git commit -m "이번 확정본에 대한 설명"
  
  실제 변경된 내용을 확정하는 명령어
  
5. git push origin master
  
  변경 내용을 원격서버로 올리는 명령
