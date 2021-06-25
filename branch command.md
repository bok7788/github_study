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
  <<<<<<< HEAD
  
  $ git log --onelog
  $ git log --all --oneline
  $ git log --all --graph --oneline
  
  (HEAD -> master)# head : 현재 속한 브랜치

- 브랜치 병합

  ```bash
  (master) $ git merge 브랜치명
  ```

  - 반드시 master 브랜치에 다른 브랜치 병합

- 브랜치 삭제

  ``` bash
  $ git branch -d 브랜치명
  ```

- 브랜치 강제 삭제

  ```bash
  $ git branch -D 브랜치명
  ```

  merge가 되지 않은 브랜치는 강제로 삭제해야함

- 1. 

- 브랜치 생성 + 이동

  ``` bash
  $ git checkout -b 브랜치명
  ```

  

  #  3가지 병합 상황

  1. fast-foward

     "다른 브랜치를 생성 한 후 master 브랜치에 변경사항이 없을 때"

  2. 3-way Merge

     "현재 브랜치(master)가 가리키는 커밋이 Merge 할 브랜치의 조상이 아니라면 깃은 현재 브랜치와 머지할 브랜치의 커밋 2개와 두 브랜치의 공통조상 하나를 사용한다."

     ### 1. 새로운 브랜치 signup 생성

     ###  2. signup 브랜치에서 signup.py # git add, commit 잊지 말자.

     ### 3. master 브랜치에서 new folder 생성

     ### 4. master 브랜치와 signup 브랜치 병합

     ### 5. signup 브랜치 삭제

  # 3. Merge Conflict

  "두개의 브랜치가 동일한 파일의 동일한 위치를 수정하고 merge하려고 할때 발생하는 현상"

  단, 동일 파일을 수정했다고 하더라도 서로 다른 영역을 수정한다면 merge conflict 는 발생하지 않는다

- 새로운 브랜치 hotfix생성

- hotfix 브랜치에서 b.txt에 새로운 내용 입력 -> git add, commit

- master 브랜치에서 b.txt 새로운 내용 입력 - > git add, commit

- master 브랜치와  hotfix  브랜치 병합

수정사항을 반영하고, add, commit 한후 log확인하면, 병합되어 있다.

$ git status

DEVPIA@DESKTOP-6JIHTHE MINGW64 ~/Desktop/github_study (master|MERGING)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 10 commits.
  (use "git push" to publish your local commits)

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   b.txt

no changes added to commit (use "git add" and/or "git commit -a")

DEVPIA@DESKTOP-6JIHTHE MINGW64 ~/Desktop/github_study (master|MERGING)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 10 commits.
  (use "git push" to publish your local commits)

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   b.txt

no changes added to commit (use "git add" and/or "git commit -a")
