# cd 명령어

## cd란?

리눅스에서 cd는 "Change Directory"의 약자로, 현재 작업 중인 디렉토리를 변경하는 데 사용됩니다.

## 사용법

사용법은 cd [디렉토리 경로] 형식으로, 이동하고자 하는 디렉토리의 경로를 입력하면 됩니다.

- **절대 경로**: `/`로 시작하는 전체 경로를 입력해 특정 디렉토리로 이동합니다.  
  예) `cd /home/user/projects`
  
- **상대 경로**: 현재 디렉토리를 기준으로 이동합니다.  
  예) `cd ../documents` (상위 디렉토리의 `documents`로 이동)

- **특수 경로 기호**:
  - `.`: 현재 디렉토리
  - `..`: 상위 디렉토리

## 예제

```bash
# 상대경로 이동
cd newFolder2
```

```bash
# 절대 경로를 사용해 이동
cd /jinseob/newFolder2
```

```bash
# 상위 디렉토리로 이동
cd ..
```

## 주의 사항

- 경로가 올바르지 않으면 `bash : cd: [디렉토리 경로]: no file or directory` 오류가 발생합니다.

- directory가 아닐 경우 `bash: cd: not directory` 오류가 발생합니다.
