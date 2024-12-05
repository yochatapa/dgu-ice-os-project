# rm 명령어

## rm이란?

리눅스에서 `rm`은 "Remove"의 약자로, 파일이나 디렉토리를 삭제하는 데 사용됩니다.  
디렉토리 삭제 시에는 옵션을 반드시 지정해야 하며, 복구가 어려우므로 신중히 사용해야 합니다.

## 사용법

사용법은 `rm [옵션] [파일/디렉토리 경로]` 형식으로, 삭제할 대상과 동작 방식을 설정할 수 있습니다.

- **옵션**:
  - `-r`: 디렉토리를 포함한 하위 파일 및 디렉토리를 재귀적으로 삭제합니다.

## 예제

```bash
# 단일 파일 삭제 (상대경로)
rm newFile
```

![rm_delete_file_relative_path](/assets/rm/rm_delete_file_relative_path.png)

```bash
# 단일 파일 삭제 (절대경로)
rm /jinseob/newFolder/newFile3.txt
```

![rm_delete_file_absolute_path](/assets/rm/rm_delete_file_absolute_path.png)


```bash
# 디렉토리 및 하위 내용 삭제
rm -r newFolder
```

![rm_r_option_delete_entire_directory](/assets/rm/rm_r_option_delete_entire_directory.png)


## 주의사항
- `-r`옵션이 없이 디렉토리를 삭제할 수 없습니다.
- 파일 삭제 전 목록을 확인하려면 ls 명령어를 함께 사용하세요.
