# Hands on Git
- 기간
  - 11/22 ~ 11/26
- 매일 오후 8시 ~ 모각코(예시)

> 질문 사항은 이슈 탭에 등록하거나 슬랙으로

> level1, level2에서 공부, 실습, 구현한 내용을 Wiki 탭에서 문서로 작성해주세요.


## level1
### Basic

1. 현재 저장소 fork
2. 로컬 저장소 세팅
3. 메인 저장소와 내 저장소(fork한 저장소) 싱크
4. 내 저장소에서 브랜치 만들기
5. `Git 공부내용_이름.md` 마크다운 파일 작성
6. add/commit/push 후 main 브랜치에 merge
7. 내 저장소에서 메인 저장소에 Pull Request & Merge
8. github issue 페이지에 완료했다고 코멘트 달기

### Advanced

1. 메인 저장소에 다른 사람들의 작업물이 올라온 후, 로컬에서 fetch pull/rebase
2. 임의의 추가작업 (위의 마크다운 파일 보충 등)
3. PR&Merge
4. Conflict 발생 시 reset, revert, cherry-pick 등 사용해서 충돌 해결
5. github issue 페이지에 완료했다고 코멘트 달기

## level2

- 깃 명령어 구현
    - 각자 사용하는 고급언어의 파일 I/O 기능을 이용
    - git 명령어들의 동작 방식을 개념적으로 구현
    - init/add/commit/push 구현
        - init
            - 작업 폴더를 만든다.
        - status
            - staging area
                - add한 파일들
            - working directory
                - 작업하는 폴더의 파일들
                - modified, unmodified
                    - 수정되었는지 표시
            - 위의 상태를 출력
        - add
            - staging area 에 복사
                - 임의의 폴더를 만들고 복사
            - `add {파일이름}`
                - 파일을 수정했으면은 다시 add했을 때 덮어쓰기
                - 바뀐 사항만 추가했을 때
        - commit
            - staging area를 비운다.
        - restore
            - git restore —staged {filename}: Staging Area에서 내려오기
            - git restore {filename}: modified → unmodified 바꾸기
    
