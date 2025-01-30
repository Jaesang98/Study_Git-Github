## 🔀 part1-5 다양한 git merge 방법 (3-way, fast-forward, squash, rebase)
### 🔹 Merge 방식
1. **3-way merge**
   - 두 브랜치를 서로 merge할 때 사용하는 방식
   - branch를 만든 시점으로 브랜치 둘다 수정이 됬을 경우 사용된다
   
   ![](https://velog.velcdn.com/images/jaesang98/post/846fbda6-d832-47ad-b73a-25c7b709842b/image.png)


2. **Fast-forward merge**
   - 한쪽 브랜치만 변경된 경우 사용하는 방식
   - branch를 merge하는것이아닌 main으로 이름을 바꾸어 쭉 이어나가는 방식
   
   ![](https://velog.velcdn.com/images/jaesang98/post/ee011c84-d589-4fc3-b836-f3f05ba64842/image.png)
```bash
# 강제로 3-way merge
git merge --no-ff
```

3. **Rebase**
   - 브랜치의 시작점을 다른 커밋으로 이동
   - 메인 브랜치의 최근 커밋으로 옮긴 후 fast-forward를 사용하는것
   - 브랜치가 많은경우 3-way merge는 나중애 git log출력할 때 복잡하기 때문에 rebase를 사용하여 깔끔하게 로그를 확인할 수 있다
   - 단점은 conflict가 많이 나온다
   
   ![](https://velog.velcdn.com/images/jaesang98/post/e62c9659-bf19-4a53-b54d-b8de8d6070eb/image.png)


4. **Squash merge**
   - 브랜치에서 커밋했던거를 전부 합쳐서 메인에 붙이는 방식이다
   - 깃 로그를 깔끔하게 보기위해 사용한다
   
   ![](https://velog.velcdn.com/images/jaesang98/post/9dfd7c6b-6bcc-4503-a6a0-889b8a3dcc43/image.png)


### 🔹 브랜치 삭제
- 사실 branch를 merge해도 삭제되지는 않는다
```bash
# 병합된 브랜치 삭제
git branch -d 브랜치명

# 강제 삭제
git branch -D 브랜치명
```
