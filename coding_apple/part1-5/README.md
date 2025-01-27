## part1-5 다양한 git merge 방법 (3-way, fast-forward, squash, rebase)

1. 3-way merge

   - main과 생성한 branch를 서로 merge할 때 사용하는 방식
   - branch를 만든 시점으로 메인과 브랜치 둘다 수정이 됬을 경우 사용된다

2. fast-forward merge

   - main은 바뀌지 않았고 branch만 merge된 경우 사용하는 방식
   - branch를 merge하는것이아닌 main으로 이름을 바꾸어 쭉 이어나가는 방식
   - 강제로 3-way merge를 하려면 git merge --no-ff 명령어 입력

3. branch 삭제

   - 사실 branch를 merge해도 삭제되지는 않는다
   - merge한 브랜치 삭제: git branch -d 브랜치명
   - merge안한 브랜치 삭제: git branch -D 브랜치명

4. rebase

   - 신규 브랜치의 시작점을 다른 commit으로 옮기는 방식
   - 메인 브랜치의 최근 커밋으로 옮긴 후 fast-forward를 사용하는것
   - 브랜치가 많은경우 3-way merge는 나중애 git log출력할 떄 복잡하기 때문에 rebase를 사용하여 깔끔하게 로그를 확인할 수 있다
   - 단점은 conflict가 많이 나온다

5. squash and merge
   - 브랜치에서 커밋했던거를 전부 합쳐서 메인에 붙이는 방식이다
   - 깃 로그를 깔끔하게 보기위해 사용한다
