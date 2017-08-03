## Git의 특징

1. 로컬 및 원격 저장소 생성
2. 로컬 저장소에 파일 생성 및 추가
3. 수정 내역을 로컬 저장소에 저장
4. 파일 수정 내역 추적(변경사항을 체크하기 위해)
5. 원격 저장소에 제출된 수정 내역을 로컬 저장소에 적용
6. Master에 영향을 끼치지 않는 브랜치 생성
7. 브랜치 사이의 병합(Merge)
8. 브랜치를 병합하는 도중의 충돌 감지

**Git 사용 명령어는 리눅스 명령어를 사용**

```
pwd // 현재 작업위치

/c/Users/kitcoop
```


#### 이름과 이메일 등록h

```
git config --global user.name "사용자명"
git config --global user.email "사용자이메일"
```



#### 저장소 생성

```
cd .. // 하위로 이동
mkdir imsi
cd imsi //imsi 폴더 생성
git init // 저장소 생성
// 브랜치를 하나 생성 시켜준다. (master)
```

##### 브랜치? 공통으로 사용이 되는 파일을 각자의 영역에서 아무런 충돌없이 사용할 수 있도록 해주는 영역



#### 첫번째 커밋

```
ls // 디렉토리 안의 파일 확인
vim test.txt // test.txt 파일 생성
i // 글을 작성 하게 커서를 넣음
print("Hello world")
:wq // 파일을 저장하고 종료
```

##### 파일의 내용 확인

```
cat 경로포함 파일명
cat test.txt // 파일의 내용을 확인 할 수 있음
```

##### git add와 git commit

git add : 각자의 브랜치에서 바뀐 내용을 git에게 알려주는 역할, git에게 저장

commit : 파일에 커밋메세지를 작성하고 나서 빠져나가게 되어있다

```햣
git status // 커밋하기전 저장소의 상태를 확인
git add test.txt // 각자 작업한 파일의 내용을 git에 기록
git commit
저장할 메세지 작성
:wq
```



#### 새로운 브랜치 생성과 이동

```
git branch // 현재 생성되어 있는 브랜치 목록 확인
git branch 생성시킬 브랜치 이름
git checkout 이동할 브랜치 이름
```

```
git add // 새로추가된 파일의 경우에 한번만 지정
git commit -a // 하나 이상의 파일을 commit 설정 할때 add+commit
```

#### 브랜치를 병합

```
git merge 병합할브랜치명
```
