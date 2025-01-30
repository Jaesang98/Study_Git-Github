## 🌳 part1-10 git flow / trunk-based 브랜치 전략
### 🔹 Git Flow
- 안정적인 운영을 할 때 사용한다
- 최근 continuous delivery 이런거 한 때 유행이었는데 그런거 할 땐 적합하지 않을 수 있다

### 🔹 Git Flow 활용순서
   1. main브랜치와 dev브랜치(개발용)를 생성
   2. feature브랜치를 생성 (dev에 기능추가)
   3. feature브랜치에서 만든게 잘 되면 dev에 merge
   4. 배포를 하는 경우 dev의 release브랜치를 따로 생성 후 여러가지 테스트를 해본다
   5. 완성이 된다면 main과 dev에 merge시킨다
   6. 만약 배포 후 버그가 생긴다면 메인에서 hotfix를 하나 만들어 바로바로 수정을 한 뒤 main, dev에 머지시킨다

![](https://velog.velcdn.com/images/jaesang98/post/e69afddd-bb6a-4236-876d-9738526b38e3/image.png)


### 🔹 Trunk-based
- 코드를 한 브랜치에서만 관리하는 방식
- 기능을 추가하는 경우 main에서 브랜치를 하나 생성해서 수정 후 머지시키는 방식
- main 브랜치에 있는 코드가 뻑이나면 큰일나기 때문에 테스트나 코드리뷰를 자주해야한다

![](https://velog.velcdn.com/images/jaesang98/post/b25bc797-68fc-4fc0-8e5c-1dd90b9a8d14/image.png)

### 🔹 어떤걸 사용해야할까
- 뼈대가 잡혀있지 않고 개발진행중인건 GitFlow, 뼈대가 잡히고 유지보수를 하는건 Trunk-based
