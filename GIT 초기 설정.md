# GIT 초기 설정

커밋 작성자 설정

```bash
# 명령을 시키고자 하는 주체
# git아, 전역 설정중 유저의 email을 설정
$ git config --global user.email bok7788@kakao.com
# git아, 전역 설정중 유저의 name을 설정
$ git config --global user.name bok7788
# Ctrl + L : clear
```

- 커밋을 작성하는 사람이 누구인지 알아야 한다.

지정된 설정 확인

```bash
# 
$ git config --global -l
# $ git config --global --list
```

## Git Basic

## 로컬저장소 설정

```bash
$ git init
```

- 폴더에 git 저장소를 초기화하면, .gif 이라는 숨김폴더가 생기고

  - bash에는 (master)라는 표기가 생성된다.

- 주의사항

  - .gif폴더를 직접적으로 수정하는 일은 없을 것이다.

  - 이미 gif으로 관리하고 있는 (bash창에 master가 표기되어 있는

    폴더 내에서는 절대 git init하지 말것)

# status

```bash
# git 관리중인 폴더의 상태를 보여줘
$ git status
```

# add

```bash
$ git add 파일명
$ git add . # 현재 디렉토리 모두
$ git add a.txt
$ git add directory_name
```

- working directory 상태의 파일을  staging area상태로 변경
- 커밋을 위한 파일 및 폴더들을 추가하는 명령어

- 자동완성 : 첫자+tab

# commit

```bash
$ git commit -m "commit message" #커밋 메세지
# git commit -m "210624 | ~~"
$ git log --oneline
#(HEAD->master) 최신버전
```

- 커밋을 통해 하나의 버전으로 기록 됨
- 커밋 메세지는 현재 변경사항들을 잘 나타낼수 있도록 작성하는 것을 권장
- 커밋 목록은 git log를 통하여 확인

# MV

- mv 이전이름 새이름







