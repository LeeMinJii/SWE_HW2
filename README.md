# **GitHub와 git 사용하기**
> GitHub 주소 -> [GitHub URL](https://github.com/LeeMinJii/SWE_HW2.git)

# **init**
>새로운 저장소를 초기화하는 명령어
>- **git init**

![git init](https://user-images.githubusercontent.com/69834230/117570312-8daf6600-b104-11eb-873f-73dd53cc26ed.png)
>>새 md파일을 새로운 곳에서 열고 git init을 입력해 공간을 만들었다.  

# **config**
>Git 최초 설정을 위해 사용자 이름, 이메일, 편집기 등의 정보를 미리 설정하는 명령어
>- 이름 설정 : **git config --global user.name "이민지"**
>- 이메일 설정 : **git config --global user.email "julia7450@naver.com"**
>- 설정 확인 : **git config --list**  

![git config](https://user-images.githubusercontent.com/69834230/117570395-d9620f80-b104-11eb-8000-43afc850f7a6.png)
>>config를 통해 사용자 이름, 이메일을 등록하고 해당 내용들을 확인했다.  

# **status**
>파일 상태를 확인하는 명령어
>- **git status**
```git status를 하여 현재 commit 해야 할 것이 있는지 등의 파일 상태를 확인했다.```

![git status](https://user-images.githubusercontent.com/69834230/117570421-fa2a6500-b104-11eb-83e2-fb46ebdb7a11.png)
>> 현재 init을 이용해 새로운 저장소만 만들었으므로 만든 md파일의 상태를 확인하기 위해 status명령어를 사용하여 현재 빨간 줄 부분의 파일을 스테이징 영역에 추가해야 함을 확인했다.

# **add**
>작업 디렉토리 상의 변경 내용을 스테이징 영역에 추가하기 위해서 사용하는 명령어
>- **git add [파일이름]** : 작업 디렉토리의 변경 내용의 일부만 스테이징 영역에 넘기고 싶을 때 
>- **git add .** : 현재 디렉토리의 모든 변경 내용을 스테이징 영역으로 넘기고 싶을 때
>- **git add -A** : 작업 디렉토리 내의 모든 변경 내용을 몽땅 스테이징 영역으로 넘기고 싶을 때
>- **git add -p** : 각 변경 사항을 터미널에서 직접 눈으로 하나씩 확인하면서 스테이징 영역으로 넘기거나 또는 제외하고 싶을 때  

![git add](https://user-images.githubusercontent.com/69834230/117570440-1a5a2400-b105-11eb-84d9-fd42edb7168d.png)
>>add -A옵션을 이용하여 지금까지 작업한 모든 파일에 대한 변경 내용을 스테이징 영역에 추가했다.

# **commit**
>변경 사항을 확정하는 명령어
>- **git commit -m "메세지"** : 인라인 형식으로 바로 커밋 메세지 작성
>- **git commit -a** : 별도의 add명령어를 사용하지 않고 수정된 파일에 대해 add, commit을 한번에 수행
>- **git commit -am "메세지"** : a, m의 옵션을 합친 형태  

![git commit](https://user-images.githubusercontent.com/69834230/117570488-3fe72d80-b105-11eb-988b-e25f1674af08.png)
>>commit -m 옵션을 이용해 앞서 add로 모든 변경 내용에 대한 커밋 메시지를 추가했다.  

# **log**
>커밋 기록을 조회하는 명령어
>- **git log** : 기본 사용
>- **git log -[숫자]** : 커밋 결과를 최근 [숫자]개의 개수만큼 보여줌  

![log](https://user-images.githubusercontent.com/69834230/117570514-5beacf00-b105-11eb-9344-f8246cdc48ff.png)  
>>지금까지 commit을 한 내역을 조회했다.  
  
# **reset --hard**
>해당 커밋 주소로 되돌아가는 명령어
>- **git reset [주소] --hard** : 돌아가려는 이력이후의 모든 내용을 지움
> (**git log**를 이용해 커밋의 주소를 확인한다.)

![git reset --hard](https://user-images.githubusercontent.com/69834230/117570630-e9c6ba00-b105-11eb-81bd-26da6ac4e2ba.png)  
>> 먼저 commit주소를 알기 위해 git log를 했다. 조회된 것들 중에 주소 부분의 앞 6자리만 따와서 [주소] 부분에 넣고 reset명령어를 이용하여 해당 commit으로 돌아가고 돌아간 부분 이후의 모든 내용은 지웠다.  

# **branch**
>독립적으로 어떤 작업을 진행하기 위한 브랜치를 만드는 명령어
>- **git branch [브랜치이름]** : 브랜치 생성
>- **git branch -D [브랜치이름]** : 브랜치 삭제

# **checkout**
>

![git branch, checkout](https://user-images.githubusercontent.com/69834230/117570673-20043980-b106-11eb-91b6-2378bdb614ea.png)

# **merge**
![git merge](https://user-images.githubusercontent.com/69834230/117571064-e7fdf600-b107-11eb-8eda-4552dcc2033f.png)

![git rebase](https://user-images.githubusercontent.com/69834230/117572166-96a43580-b10c-11eb-8317-44b92bdcc34a.png)

![git remote, pull](https://user-images.githubusercontent.com/69834230/117573032-c8b79680-b110-11eb-9c38-b220d2903a35.png)

![git push](https://user-images.githubusercontent.com/69834230/117573075-f7357180-b110-11eb-9284-e96f3b25a7c9.png)

![git clone](https://user-images.githubusercontent.com/69834230/117573100-116f4f80-b111-11eb-9d91-cf76d2a8c258.png)

![git tag1](https://user-images.githubusercontent.com/69834230/117573120-2fd54b00-b111-11eb-88e6-f370eb92e87d.png)

![git tag2](https://user-images.githubusercontent.com/69834230/117573138-50050a00-b111-11eb-966d-d658dc53fd87.png)

|     명령어       |       사용여부      |
|-----------------|---------------------|
|[init](#init)|          O          |
|[add](#add)  |          O          |
|[config](#config)|      O          |
|[log](#log)|            O          |
|[status](#status)|      O          |
|[commit](#commit)|      O          |
|[branch](#branch)|      O          |
|[checkout](#checkout)|      O      |
|[merge](#merge)|        O          |
|[reset --hard](#reset---hard)|        O          |
|[rebase](#rebase)|      O          |
[remote](#remote)|       O          | 
|[push](#push)|          O          |
|[pull](#pull)|           O          |
|[clone](#clone)|         O          |
|[tag](#tag)|             O          |
