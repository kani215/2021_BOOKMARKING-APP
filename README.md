# 2021_BOOKMARKING-APP
커맨드라인용 북마크 앱을 만들어보았습니다.

# 1. 간단 소개

> 애플리케이션 :

READ : 기존의 북마크 정보 모든 북마크 목록, 어떤 조건에 맞는 특정 북마크를 얻는다.
UPDATE : 제목 또는 메모와 같은 북마크의 정보를 수정한다.
DELETE : 북마크를 제거한다.

> 기능 :

- 아이디 - 북마크의 고유한 숫자 식별자
- 제목 - 북마크에 대한 짧은 텍스트 제목
- URL - 저장 중인 기사 또는 웹사이트에 대한 링크
- 메모 - 선택 사항으로 북마크에 대한 긴 설명
- 추가한 날짜 - 북마크의 최신도 타임스탬프 기능 위함
- CLI를 통해서 처리되게 설정

# 2. 초기 코드 구조

- 커맨드라인 인터페이스 - 사용자에게 메뉴 옵션을 제공
- 메뉴 옵션 선택 - 사용자의 선택에 따라 알고리즘 작동이 다르다.
- DB 저장 - DB에 기본 정보는 저장되어 있음 DB 기능은 영구적 활용 가능하게 캡슐화 해서 작성 예정
- DB는 SQLITE를 사용한다. [https://wikidocs.net/12454](https://wikidocs.net/12454)

# 3. Readme

- src

    [commands.py](https://github.com/kani215/2021_BOOKMARKING-APP/blob/main/src/commands.py) # db 언어를 조작 명령

    [database.py](https://github.com/kani215/2021_BOOKMARKING-APP/blob/main/src/database.py) #sql 언어들로 db를 조작하는 파일

    [main.py](https://github.com/kani215/2021_BOOKMARKING-APP/blob/main/src/main.py) #전체 파일을 실행

bookmarks.db # sqlite db 파일에 저장
