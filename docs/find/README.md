# find 명령어

## find란?

리눅스에서 `find`는 파일 및 디렉토리를 검색하는 명령어로, 지정된 경로와 조건에 따라 원하는 파일이나 디렉토리를 찾을 수 있습니다.

## 사용법

사용법은 `find [검색 경로] [조건]` 형식으로, 검색할 경로와 조건을 설정합니다.  
**특이사항**: `-name`과 `-type` 옵션은 독립적으로 사용해야 합니다.

- **주요 옵션**:
  - `-name [패턴]`: 이름이 지정된 패턴과 일치하는 파일이나 디렉토리를 찾습니다.  
    (패턴에 와일드카드(`*`)를 사용할 수 있습니다.)
  - `-type [종류]`: 파일 타입을 지정합니다.  
    - `f`: 일반 파일  
    - `d`: 디렉토리  

## 예제

```bash
# 현재 디렉토리에서 이름이 'file.txt'인 파일 검색
find . -name "file.txt"
```

```bash
# 특정 경로에서 이름에 'log'가 포함된 파일 검색
find /var/logs -name "*log*"
```

```bash
# 현재 디렉토리에서 일반 파일만 검색
find . -type f
```

```bash
# 홈 디렉토리에서 디렉토리만 검색
find / -type d
```

## 주의 사항
- 옵션 -name과 -type은 독립적으로 사용해야 하며, 함께 작성하면 오류가 발생합니다.
- 검색 경로를 생략하면 기본적으로 현재 디렉토리(.)를 기준으로 검색합니다.
