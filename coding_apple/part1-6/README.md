## ⏮️ part1-6 코드짜다가 실수했다 되돌아가자 (git revert, reset, restore)
### 🔹 파일 복구 (restore)
```bash
# 최근 커밋 상태로 복구
git restore 파일명

# 특정 커밋 시점으로 복구
git restore --source 커밋ID 파일명

# Staging 취소
git restore --staged 파일명
```

### 🔹 커밋 취소 (revert)
```bash
# 특정 커밋 취소
git revert 커밋ID

# 최근 커밋 취소
git revert HEAD
```

### 🔹 커밋 리셋 (reset)
```bash
# 완전히 되돌리기
git reset --hard 커밋ID

# 변경사항 스테이징 유지
git reset --soft 커밋ID

# 변경사항 언스테이징
git reset --mixed 커밋ID
```
