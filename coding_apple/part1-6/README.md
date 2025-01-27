## part1-6 코드짜다가 실수했다 되돌아가자 (git revert, reset, restore)

1. git restore

   - git restore 파일명 : 파일을 최근 커밋상태로 복구할 때 사용한다
   - git restore --source 커밋아이디 파일명 : 커밋 아이디 시점으로 파일을 복구한다
   - git restore --staged 파일명 : add한파일을 취소해준다

2. git revert

   - git revert 커밋아이디 : 커밋한 내용을 취소할 때 사용한다
   - git revert HEAD : 최근 commit한 내용을 취소할 때 사용한다

3. git reset
   - git reset --hard 커밋아이디 : 커밋한 시점으로 모든 파일을 되돌린다
   - git reset --soft 커밋아이디 : 커밋한 시점으로 모든 파일을 되돌리며 변경사항은 스테이징해놓음
   - git reset --mixed 커밋아이디 : 커밋한 시점으로 모든 파일을 되돌리며 변경사항은 언스테이징해놓음
