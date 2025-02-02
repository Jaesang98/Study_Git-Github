## 📦 part1-11 git stash로 코드 잠깐 보관하기

### 🔹 Stash

- 수정했던 코드들을 잠시 다른곳에 보관하고 싶을 때 사용한다

### 🔹 Stash 명령어

```bash
# 변경사항 임시 저장
git stash
git stash save "메모"

# Stash 목록 확인
git stash list

# 보관했던 코드들을 전부 가져옴 (다만 가장 최근에 보관한것 순으로 가져온다)
git stash pop

# Stash 삭제
git stash drop stash@{n}

# 모든 stash삭제
git stash clear
```
