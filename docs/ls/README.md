# ls 명령어

## ls란?

리눅스에서 `ls`는 현재 디렉토리의 파일 및 디렉토리 목록을 출력하는 명령어입니다. 파일 탐색이나 디렉토리 구조 확인 시 가장 자주 사용됩니다.

## 사용법

사용법은 `ls [옵션] [디렉토리 경로]` 형식으로, 출력 방식과 대상 디렉토리를 설정할 수 있습니다.

- **디렉토리 경로**: 특정 경로를 지정하지 않으면 기본적으로 현재 디렉토리의 내용을 출력합니다.

- **주요 옵션**:
  - `-a`: 숨김 파일(`.`으로 시작하는 파일)을 포함한 모든 파일을 표시합니다.
  - `-l`: 파일의 상세 정보(권한, 소유자, 크기, 수정 시간 등)를 출력합니다.
  - `-la` 또는 `-al`: 숨김 파일을 포함한 모든 파일을 상세 정보와 함께 표시합니다.

## 예제

```bash
# 현재 디렉토리의 파일과 디렉토리 출력
ls
```

![ls_check_current_folder](/assets/ls/ls_check_current_folder.png)

```bash
# 특정 상대경로의 파일과 디렉토리 출력
ls newFolder2
```

![ls_check_relative_path_folder](/assets/ls/ls_check_relative_path_folder.png)

```bash
# 특정 절대경로의 파일과 디렉토리 출력
ls /jinseob/newFolder2
```

![ls_check_absolute_path_folder](/assets/ls/ls_check_absolute_path_folder.png)

```bash
# 숨김 파일을 포함한 모든 파일 출력
ls -a
```

![ls_a_option_show_hidden_files](/assets/ls/ls_a_option_show_hidden_files.png)

```bash
# 파일의 상세 정보를 출력
ls -l
```

![ls_l_option_detailed_file_info](/assets/ls/ls_l_option_detailed_file_info.png)

```bash
# 숨김 파일을 포함하여 상세 정보 출력
ls -la
ls -al
```
![ls_la_al_options_combined](/assets/ls/ls_la_al_options_combined.png)