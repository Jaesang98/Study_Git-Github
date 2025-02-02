## 🖥️ part1-3 git add, commit, diff 쉽게 하는 법 (VSCode)

### 🔹 VSCode를 통한 Git 관리

- 요즘은 에디터에 git기능이 내장되어있어 굳이 명령어를 사용 할 필요는 없다.
- Source Control 탭을 통해 직관적인 Git 작업 가능
- 변경사항 시각적 확인 용이

### 🔹 git diff

- 파일이 수정되었을 때 어떤내용이 수정되었는지를 보기 위한 명령어
- 터미널로 보기 때문에 가독성이 많이 떨어지고 버그도 많아서 사용은 잘 안한다.

```bash
# 변경사항 확인
git diff
```

### 🔹 git difftool

- git diff대신하여 vim 에디터를 통해서 차이점을 볼 수 있음
- 사실 비교해주는 에디터들이 있기때문에 잘 사용하지 않는다

```bash
# Vim을 통한 차이점 확인
git difftool 커밋ID
git difftool 커밋ID1 커밋ID2
```
