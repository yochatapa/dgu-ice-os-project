# mkdir 명령어

## mkdir이란?

리눅스에서 `mkdir`은 "Make Directory"의 약자로, 새로운 디렉토리를 생성하는 데 사용됩니다.

## 사용법

사용법은 `mkdir [옵션] [디렉토리 이름]` 형식으로, 생성하려는 디렉토리 이름과 필요한 옵션을 입력합니다.

- **디렉토리 이름**: 생성할 디렉토리의 이름 또는 경로를 지정합니다.

- **옵션**:
  - `-m`: 생성되는 디렉토리의 권한을 설정합니다.  
    예) `mkdir -m 755 newFolder` (읽기, 쓰기, 실행 권한을 설정한 디렉토리 생성)
  - `-p`: 상위 디렉토리가 없는 경우 상위 디렉토리까지 한 번에 생성합니다.  
    예) `mkdir -p /home/user/projects/newFolder`

## 예제

```bash
# 단일 디렉토리 생성
mkdir newFolder
```

![mkdir_relative_path](/assets/mkdir/mkdir_relative_path.png)

```bash
# 디렉토리 생성 (절대경로)
mkdir /jinseob/newFolder2
```

![mkdir_absolute_path](/assets/mkdir/mkdir_absolute_path.png)

```bash
# 권한을 설정하여 디렉토리 생성
mkdir -m 777 mOption
```

![mkdir_with_m_option](/assets/mkdir/mkdir_with_m_option.png)

```bash
# 상위 디렉토리를 포함하여 생성
mkdir -p pOption/newP1
```

![mkdir_create_subdirectory_with_p_option_success](/assets/mkdir/mkdir_create_subdirectory_with_p_option_success.png)

```bash
# 여러 디렉토리 동시에 생성
mkdir multi1 multi2
```

![mkdir_create_multiple_folders_simultaneously](/assets/mkdir/mkdir_create_multiple_folders_simultaneously.png)

## 주의사항

- root 폴더 생성 시 `mkdir : [디렉토리 이름] can't make directory: deny permission` 오류가 발생합니다.
- 이미 동일한 이름의 디렉토리가 존재하면 `mkdir: mkdir :can't make [디렉토리 이름]: already have file` 오류가 발생합니다.
- p 옵션을 사용하면 상위 디렉토리가 이미 존재해도 오류 없이 작업을 수행합니다.
