## part1-2 git add, commit으로 파일 기록해놓을 수 있음

1. git 사용법

   1. 작업폴더에 git init입력
      => git이라는 소프트웨어가 파일생성 및 코드 작성하는걸 감시함

   2. git add, commit

      - git add 파일명
      - git commit -m '아무메세지'
        => 커밋 기록을 한다

      * 두번의 명령어를 쓰는 이유는 add를 통해 기록을 할 파일을 걸러낸 후 commit을 통해 기록을 한다고 생각하면 된다 \*

   3. staging
      - git add된 파일들이 있는 장소를 staging
      - git commit된 파일들이 있는 장소를 repository(저장소) 라고한다

2. 유요한 명령어
   - git add . (모든 파일을 staging)
   - git status (어떤 파일이 staging 및 수정이되있는지를 알려준다)
   - git log --all --oneline (commit한 내역을 조회한다)
