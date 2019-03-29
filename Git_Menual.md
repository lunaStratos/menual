# Git 간단 설명

## 초기설정

1. git init

git 초기 등록

2. git remote add origin [address]

> ex: git remote add origin https://github.com/lunaStratos/menual.git



## commit & push

1. git add *

전체 대기열에 올리기

2. git commit -m "메시지"

메시지에 변경사항 적기

3. git push origin master

잘 안되면 -f를 추가하면 강제로 업로드 가능

> ex: git push origin master -f


## Git 무시목록(.gitignore ) 설정

일반적인 템플릿은 https://www.gitignore.io/ 에서 찾아서 입력

폴더처리 
config/api.js
압축파일 처리
*.zip

이후 아래 커맨드 적용 

> git rm -r --cached .
> $ git add .
> $ git commit -m "fixed untracked files"
