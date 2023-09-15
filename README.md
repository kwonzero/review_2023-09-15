# review_2023-09-15

## GOAL

- 코드 관리를 위한 git의 정확한 사용법을 이해한다.

- git의 저장소 개념을 이해하고, 원격 저장소 서비스의 차이를 인식한다.

- git을 사용하면서 발생하는 다양한 상황을 해결할 수 있다.

- commit의 보편적인 작성법을 이해하고 이를 활용하여 commit을 작성할 수 있다.

- git의 branch model을 활용해 능숙하게 코드관리할 수 있다.

- git의 다양한 branch 전략을 이해하고 널리 사용되는 git flow 전략을 활용하여 프로젝트를 수행할 수 있
다.

- github projects와 issue로 프로젝트 이슈를 관리할 수 있다.

- git으로 타인과 협업하며, 다른 프로젝트에 기여할 수 있다.

---

# Shell Command

- $ ls
- $ cd Documents
- $ mkdir dev
- $ pwd

- $ touch newfie.md
- $ mv newfile.md temp/
- $ cp newfile.md newfile_copy.md
- $ rm newfile.md
- $ rm -rf temp
- $ cat newfile.md

---

# Vim Command



## normal mode

- h j k l - left, down, up, right
- i - insert mode
- v - visual mode
- ESC - back to normal mode
- d - delete
- dd - delete a line
- y - yank
- yy - yank a line
- p - paste
- u - undo
- a - append
- A - append from end of line
- o - open line(under)
- O - open line(upper)
- H - move to the top of the screen
- L - move to the bottom of the screen



## Cmd-line mode

- :q - quit

- :q! - override and quit

- :w - write

- :wq - write and quit

- :{num} - Go to {num}th line

---

# Pros

- 소스코드 주고받기 없이 동시작업이 가능해져 생산성이 증가

- 수정내용은 commit 단위로 관리, 배포 뿐 아니라 원하는 시점으로 Checkout 가능

- 새로운 기능 추가는 Branch로 개발하여 편안한 실험이 가능하며, 성공적으로 개발이 완
료되면 Merge하여 반영

- 인터넷이 연결되지 않아도 개발할 수 있음

---

# Git Internals - objects

- Blob: 파일 하나의 내용에 대한 정보

- Tree: Blob이나 subtree의 메타데이터(디렉토리 위치, 속성, 이름 등)

- Commit: 커밋 순간의 스냅샷
![HEROPY](https://git-scm.com/book/en/v2/images/data-model-1.png)

---

# Git Local and Remote Repository

![HEROPY](https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3963/10395.png)

---

# How to start

- $ git clone {username/repo-addr}
- $ cd {repo adrr}
- $ ci README.md
- $ git status
- $ git add README.md
- $ git commit
- $ git push origin main

---

# Conventional Commits
[Conventional Commit 자세한 설명](https://www.conventionalcommits.org/ko/v1.0.0/)


1. commit의 제목은 commit을 설명하는 문장형이 아닌 구나 절의 형태로 작성

2. importanceofcapitalize `Importance of Capitalize`

3. prefix 꼭 달기

    - feat: 기능 개발 관련

    - fix: 오류 개선 혹은 버그 패치

    - docs: 문서화 작업

    - test: test 관련

    - conf: 환경설정 관련

    - build: 빌드 작업 관련

    - ci: Continuous Integration 관련

    - chore: 패키지 매니저, 스크립트 등

    - style: 코드 포매팅 관련


## Conventional Commit - templete

- {type}: {description} 작업단위 축약(breaking change가 있다면 type 뒤에 !)

- {body} 작업 상세 기술

- {footer} 부가정보(ex) BREAKING CHANGE: Drop email sign up support)


---

# README.md
[FastAPI](https://github.com/tiangolo/fastapi)

```html
# ProjectName

This is Abstract. See [Demo](Demo link)

Project badges(CI/CD, gh stars, ..)

## Prerequisites

## How to Start

## Installation

## Features

## Run Tests(optional)

## Credit
```

---

# .gitignore
- 특정 파일이나 디렉토리를 추적하지 않도록 명시하기 위한 파일  
[gitignore.io](https://gitignore.io/)



0 comments on commit aafb4c0
@kwonzero
 
Leave a comment
선택된 파일 없음
Attach files by dragging & dropping, selecting or pasting them.
 You’re receiving notifications because you’re watching this repository.
Footer
© 2023 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
feat: Write a 2023-09-15 recture review · kwonzero/review_2023-09-15@aafb4c0
