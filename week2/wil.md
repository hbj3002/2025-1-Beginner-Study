# 2주차 정리
***
## Fork
다른 사용자의 레포지토리를 자신의 레포지토리로 복사하여 수정 및 관리 하는 기능

## Star
git의 북마크와 기능으로 레포지토리나 프로젝트에 Star을 달아 관리가 가능해진다.

## Issue

Repository에서 작업 계획, 버그, 추가 기능 요청 등을 기록 및 관리 하는데 사용
to-do-list 와 유사
## Branch

기존 브랜치에서 분기되어 생성되는 별도의 작업 공간

## Pull Request

분기된 Branch를 다시 병합하기 위한 절차

## Merge

### Merge commit

기본 Merge 방식이다. 새로운 커밋을 추가해서 브랜치를 합친다.

장점:

히스토리를 보존해서 변경 사항을 추적하기 쉬움.

모든 커밋이 그대로 남아있어서 팀 작업 히스토리 유지 가능.

 단점:

커밋 히스토리가 복잡해질 수 있음.
### Squash and Merge
브랜치의 모든 커밋을 하나의 커밋으로 합쳐서 main에 Merge

기존 브랜치의 개별 커밋은 사라지고, 하나의 커밋으로 깔끔하게 정리됨.

장점:

커밋 히스토리가 깔끔해짐

단점:

개별 커밋이 사라지므로 세부 변경 사항을 나중에 확인하기 어려움

### Rebase and Merge

A, B, C 커밋의 base를 재설정, 모두 새로운 커밋으로 변경

장점:

커밋 히스토리가 직선형(linear)으로 정리됨

git log가 깔끔해서 변경 사항을 쉽게 추적 가능

단점:

리베이스 과정에서 충돌(conflict) 발생 가능

***
세가지 방식으로 나오는 결과는 같지만, 커밋 히스토리 관리 방식이 달라진다. 

결론적으로, 

Merge Commit: 브랜치의 병합 과정을 명확하게 남기고 싶을 때

Squash and Merge: 작업 기록을 하나의 커밋으로 깔끔하게 정리

Rebase and Merge: 커밋 개별 유지하면서도 히스토리를 직선형으로 정리

이렇게 정리할 수 있다.
## branch 명령어 모음

### 브랜치 확인/모두 확인
$git branch 

$git branch -a

### 브랜치 생성/삭제

$git branch "<브랜치 이름>"

$git branch -D "<브랜치 이름>"

### 브랜치 이동/생성 후 이동

$git checkout “<브랜치 이름>”

$git checkout -b “<브랜치 이름>

*** 
실습 과제

https://github.com/hbj3002/2025-1-Beginner-Study/pull/2