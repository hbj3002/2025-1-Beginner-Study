## 1주차 정리
***

#  git이 필요한 이유

- 코드 수정 이력 관리
- 다수의 파일 관리
- 코드 협업 및 동기화

# 파일의 생명주기

크게 Untracked 와 Tracked로 나뉘고 Tracked는 다시  Unmodified, Modified, Staged 로 나누어 진다.
untracked인 파일을 깃으로 관리하기 위해 등록하면 tracked 상태가 되고, 이 파일을 제거(remove)하기 전 까지, Unmodified, Modified, Staged 3가지 주기를 돌게 된다. 

# git 의 영역
Working Directory: 
현재 작업 중인 파일들이 있는 공간

Staging Area: 
Commit 하기 전 변경사항을 임시 저장하는 영역

Local Repository:
git commit -m 명령어로 깃에 반영

