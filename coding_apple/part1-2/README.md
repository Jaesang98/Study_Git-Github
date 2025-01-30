## 📂 part1-2 git add, commit으로 파일 기록해놓을 수 있음
### 🔹 기본 사용법
```bash
# git이라는 소프트웨어가 파일생성 및 코드 작성하는걸 감시함
git init

# 파일 스테이징
git add 파일명
git add .  # 모든 파일 스테이징

# 변경사항 커밋
git commit -m '커밋 메시지'
```

### 🔹 Staging
- git add된 파일들이 있는 장소를 staging이라 한다
- git commit된 파일들이 있는 장소를 repository(저장소) 라고한다

### 🔹 유용한 명령어
```bash
# 상태 확인
git status

# 커밋 이력 조회
git log --all --oneline
```
