# 3주차 정리

## 사전 지식


### git log

커밋 기록을 최신 순으로 확인\
--oneline 옵션으로 간략히 표시

### Commit Id

commit의 식별을 위해 사용하는 40자 길이의 16진수

### HEAD

현재 작업 중인 브랜치의 최신 커밋을 가리킴\
새로운 커밋 생성 시 HEAD도 이동

### git status

파일 상태 확인\
(Staging Area, Working Directory, Untracked)

## 커밋 되돌리기

### commit --amend

마지막 커밋 수정

완전히 새로운 commit으로 대체 -> 커밋 ID 변경됨


(주의: 공유된 커밋은 amend 금지)

ex)\
$git commit --amend -m “커밋 메시지":\
vim 진입 없이 commit 메시지 수정

$git commit --amend --no-edit:\
메시지 수정 없이 commit 수정

### reset

커밋을 지정된 상태로 되돌림\
3가지 옵션(soft, mixed, hard)

옵션별 차이:

--soft: Staging Area로 이동\
--mixed (기본값): Working Directory로 이동\
--hard: 변경 사항 완전 삭제

### revert

커밋을 삭제하지 않고 되돌리는 새 커밋 생성.

$git revert <commit_id>: 기본\
$git revert --no-edit <commit_id>: 편집기 진입 없이 바로 revert\
$git revert --no-commit: 직접 commit 하지 않고, revert 내용을 Staging Area에 올림