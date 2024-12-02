# dgu-ice-os-project

## 프로젝트 정보

동국대학교 컴퓨터공학부 정보통신공학전공
"운영체제" 과목 실습 과제

### 과제 : Mini Operating System을 구현하라. 

[상세 지침](./docs/GuideLine.md)

### Mini Operating System이란?

Mini Operating System은 다양한 자료구조를 활용하여 리눅스 CLI(Command Line Interface)를 클론 코딩하는 프로젝트입니다.
이 프로젝트에서는 ls, cd, mkdir, rm 등 주요 명령어를 직접 구현하며, 멀티프로세서를 설계하여 여러 명령어가 동시에 동작할 수 있도록 개발하는 것이 목표입니다.

<br>

### How To Use

1. src 폴더에 있는 main.c를 다운받습니다.
2. 실행시킬 `Linux` 환경에 `main.c`를 위치시킵니다.
3. main.c를 컴파일해줍니다.
```sh
    gcc -std=c99 -o 실행파일명 main.c
```
4. 실행파일을 실행시켜줍니다.
```sh
    ./실행파일명
```