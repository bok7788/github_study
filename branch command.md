# branch command

- 브랜치 생성

  ``` bash
  $ git branch 브랜치명
  ```

- 브랜치 목록

  ``` bash
  $ git branch
  ```

- 브랜치 이동

  ``` bash
  # git checkout 까지입력 tab두번
  $ git checkout 브랜치명
  
  $ git log --onelog
  $ git log --all --oneline
  $ git log --all --graph --oneline
  
  (HEAD -> master)# head : 현재 속한 브랜치
  ```

- 브랜치 생성 + 이동

  ```bash
  $ git checkout -b 브랜치명
  ```

- 브랜치 병합