# 원격저장소(remote repository)

## 기본설정

1. 로컬 git 저장소 준비
2. github repository 생성
3. Repository default branch 변경

# 명령어

### 원격 저장소 주소 추가

```bash
# git 원격 저장소 추가 name : origin
$ git remote add origin https://github.com/bok7788/github_study.git
```

### 원격저장소 목록 확인

```bash
$ git remote -v
```

### 원격 저장소 삭제

```bash
$ git remote rm origin
```

### 원격 저장소에 업로드(push)

```bash
# origin 원격저장소에 master브랜치에 commit 내용 업로드
$ git push -u origin master
```

# github에서 소스 가져오기

- 원격 저장소 내용 전체 복제
- 주의사항 : 이미 git init 되어 있음

```bash
$ git clone {원격저장소 url}
```



# 원격 저장소의 변경사항 받아옴(update)

```bash
$ git pull origin master
```

