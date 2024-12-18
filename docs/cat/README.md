# cat 명령어

## cat이란?

리눅스에서 `cat`은 "Concatenate"의 약자로, 파일의 내용을 출력하거나, 여러 파일을 결합하는 데 사용되는 명령어입니다.
(본 프로젝트에서는 파일 결합은 개발되어 있지 않습니다.)
간단한 파일 생성이나 내용 확인 작업에서도 유용하게 쓰입니다.

## 사용법

사용법은 `cat [옵션] [파일 경로]` 형식으로, 파일의 내용을 출력하거나 특정 작업을 수행할 수 있습니다.

- **주요 옵션**:
  - `>`: 지정한 파일을 새로 생성하고, 표준 입력으로 받은 내용을 해당 파일에 저장합니다.
  - `-n`: 출력 시 각 줄에 줄 번호를 함께 표시합니다.

## 예제

```bash
# 새 파일 생성 및 내용 입력 (상대경로)
cat >newFile
# 입력할 내용 작성 후 end로 저장 종료
```

![cat_create_file_relative_path](/assets/cat/cat_create_file_relative_path.png)

```bash
# 새 파일 생성 및 내용 입력 (절대경로)
cat >/jinseob/newFolder/newFile2
# 입력할 내용 작성 후 end로 저장 종료
```

![cat_create_file_absolute_path](/assets/cat/cat_create_file_absolute_path.png)

```bash
# 파일의 내용 출력
cat newFile
```

![cat_display_file_content](/assets/cat/cat_display_file_content.png)

```bash
# 파일 내용을 출력하며 줄 번호 추가
cat -n newFile
```

![cat_n_option_with_line_numbers](/assets/cat/cat_n_option_with_line_numbers.png)

## 주의사항

- 번호는 `-n`옵션을 사용해야 출력되며, 기본적으로는 표시되지 않습니다.
