# tree 명령어

## tree란?

리눅스에서 `tree`는 디렉토리 구조를 트리 형태로 시각적으로 출력하는 명령어입니다.  
파일과 디렉토리의 계층 구조를 한눈에 확인할 수 있어 편리합니다.

## 사용법

사용법은 `tree [옵션] [디렉토리 경로]` 형식으로, 출력 형태를 제어할 수 있습니다.

- **주요 옵션**:
  - `-a`: 숨김 파일 및 디렉토리(`.`으로 시작하는 항목)를 포함하여 출력합니다.
  - `-f`: 출력 결과에 각 항목의 전체 경로를 표시합니다.
  - `-p`: 파일과 디렉토리의 권한 정보를 출력합니다.  

**특이사항**: 각 옵션은 독립적으로 작성해야 하며, `-a -f -p`처럼 옵션을 분리해야 동작합니다.

## 예제

```bash
# 현재 디렉토리의 트리 구조 출력
tree
```

```bash
# 숨김 파일을 포함하여 출력
tree -a
```

```bash
# 전체 경로를 표시하며 출력
tree -f
```

```bash
# 권한 정보를 표시하며 출력
tree -p
```

```bash
# 숨김 파일을 포함하고, 전체 경로와 권한 정보를 함께 출력
tree -a -f -p
```

```bash
# 특정 디렉토리의 트리 구조 출력
tree /home/user/projects
```