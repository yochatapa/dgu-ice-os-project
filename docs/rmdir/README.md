# rmdir 명령어

## rmdir이란?

리눅스에서 `rmdir`은 "Remove Directory"의 약자로, 디렉토리를 삭제하는 명령어입니다.

## 사용법

사용법은 `rmdir [옵션] [디렉토리 경로]` 형식으로, 삭제할 디렉토리와 동작 방식을 설정할 수 있습니다. 

- **주요 옵션**:
  - `-p`: 상위 디렉토리까지 함께 삭제합니다. 

## 예제

```bash
# 빈 디렉토리 삭제 (상대경로)
rmdir mOption
```

```bash
# 빈 디렉토리 삭제 (절대경로)
rmdir /jinseob/multi1
```

```bash
# 상위 디렉토리를 포함하여 삭제
rmdir -p aaa/bbb/ccc
```

```bash
# 여러 디렉토리 삭제
rmdir aaa/bbb/ccc aaa/ddd
```

## 주의 사항
- 디렉토리가 비어 있지 않으면 `rmdir : fail to remove directory [디렉토리 경로] : directory is not empty` 오류가 발생합니다.
- 빈 디렉토리가 아닌 경우, rm -r 명령어를 사용해야 합니다.
- `-p` 옵션을 사용할 때, 지정된 디렉토리와 상위 디렉토리 모두 비어 있어야 삭제가 가능합니다.