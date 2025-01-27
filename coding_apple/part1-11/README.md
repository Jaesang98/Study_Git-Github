## part1-11 git stash로 코드 잠깐 보관하기

1. git stash

   - 수정했던 코드들을 잠시 다른곳에 보관하고 싶을 때 사용한다

2. git stash 명령어
   - git stash : 방금 작성한 것들을 다른 공간에보관
   - git stash save "내용" : 방금 작성한 것들을 다른 공간에보관하며 메모도 함
   - git stash list : stash되있는 목록을 보여준다
   - git stash pop : 보관했던 코드들을 전부 가져옴 (다만 가장 최근에 보관한것 순으로 가져온다)
   - git stash drop 삭제할id : 특정 stash 삭제
   - git stash clear : 모든 stash삭제
