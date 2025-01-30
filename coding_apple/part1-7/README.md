## 🚀 part1-7 Github 사용법 1. 내 코드 올릴 땐 git push
### 🔹 git repostor
- git이 파일 기록해두는 장소

### 🔹 git push
- 로컬저장소를 원격 저장소로 push해준다
- 
```bash
# 코드 푸시
git push -u 저장소주소 main

# -u를 한번 붙인상태로 push를 했다면 다음 push할때는 그냥 git push만 써도된다
git push
```

### 🔹 git remote
- 긴 주소는 변수로 등록이 가능하다
```bash
# 원격 저장소 등록
# origin이라는 변수에 주소가 등록됨
git remote add origin 저장소주소
```

### 🔹 사용
```bash
# 원격 저장소 등록
git remote add origin 저장소주소

# 코드 푸시
git push -u origin main
```
