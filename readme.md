-----------------------------

#### 각오

+ 수업에 1000% 집중하기
+ 출석률 관리하기
+ 그 날 배운 내용은 꼭 복습해서 내 지식으로 만들기
+ 스터디 활용해서 반 친구들과 함께 자격증 취득하기

-------------------------------------------

#### 오늘 배운 내용

Git, vsCode, typora

CLI(Commnad Line)
/GUI(Graphic Use)

1) windows
- Git 설치 후 윈도우 탐색기를 엽니다. ( 윈도우키 + e )
- C:/사용자(Users)/현재 사용자 계정 로 이동합니다.
- 폴더 내 빈 공간에서 마우스 우클릭 후 Git Bash Here 를 클릭합니다.
- Git Bash 창에 아래 화면처럼 HOME 폴더를 의미하는 ~ 표시만 있다면 정상입니다.
( ~ 표시가 없거나, 뒤에 글자가 추가적으로 나타난다면 잘못된 경로일 수 있습니다.)


2) mac
- Spotlight (검색)를 엽니다. (화면 우측 상단의 돋보기 혹은 command + spacebar )
- terminal 을 검색하여 터미널을 엽니다.
- 터미널을 열면 기본적으로 HOME 폴더로 경로가 설정 되어 있습니다. 
   ( /Users/현재 사용자 계정 )
- open . 라고 입력하여 HOME 폴더를 엽니다.


./ :현재 작업하고 있는 폴더
../ : 현재 작업하고 있는 폴더의 부모 폴더
~: 홈디렉토리

<CLI>
cd : change directory
ls: list segments(현재 작업 중인 디렉토리의 폴더/파일 목록을 출력
mkdir: make directory
touch: 파일 생성
mv: move
rm: remove
start (open): 파일 편집기 실행


이동하고자 하는 folder 의 이름이 newfolder> 인 경우에는
mv text1.txt newfolder
이동하고자 하는 folder 의 이름이 <new folder> 인 경우에는
mv text1.txt 'new folder'
mv text1.txt "new folder"


option / 인수


유용한 단축키
위, 아래 방향키 : 과거에 작성했던 명령어 조회
tab : 폴더/파일 이름 자동 완성
ctrl + a : 커서가 맨 앞으로 이동
ctrl + e : 커서가 맨 뒤로 이동
ctrl + w : 커서가 앞 단어를 삭제
ctrl + l : 터미널 화면을 깨끗하게 청소 (스크롤 올리면 과거 내역 조회 가능)
ctrl + insert : 복사
shift + insert : 붙여넣기


파이썬 언어를 개발하기위한 개발 환경:
  .py : 메모장으로 텍스트 파일 => interpreter/파이썬
  .hwp/.doc/.mp3/.jpg : 메모장
  vsCode / 파이참

마크다운:
   일반 테스트 기반의 (경량) 마크업 언어
   .md


장점: 직관적이고 쉽다.
        관리가 쉽다.
        지원 가능한 플랫폼, 프로그램 다양하다.
        
단점: 표준이 없다.
        HTML 마트업 기능을 대신하지는 못한다.

git 명령어

working directory: 로컬의 사용자 작업이 일어나는 곳
staging area: 커믹을 위한 파일 및 폴더가 추가되는 곳
repository(commits): 변경사항(커밋)을 저장하는 곳

1) 커밋기록자를 등록
git config --global user.name ""
git config --global user.email ""

git config --global -l
git config --global --list

2) local directory를 git으로 관리한다고 정의
git init

3) git 상태 표시
   git status

   - untracked: git 이 관리하지 않는 파일
   - tracked: git이 관리하는 파일

--- file 생성( touch a.txt)
4) git add(staging)
git add 파일이름(폴더이름/)
git add .   => 전체 다

5) git commit
git commit -m "메시지"

6) git log (commit log)
--oneline : 한 줄로 축약해서 보여줍니다.
--graph : 브랜치와 머지 내역을 그래프로 보여줍니다.
--all : 현재 브랜치를 포함한 모든 브랜치의 내역을 보여줍니다.
--reverse : 커밋 내역의 순서를 반대로 보여줍니다. (최신이 가장 아래)
-p : 파일의 변경 내용도 같이 보여줍니다.
-2 : 원하는 갯수 만큼의 내역을 보여줍니다. (2 말고 임의의 숫자 사용 가능)

7) 원격 저장소 등록
git remote add <이름><주소>
    * 보통 remote연결이 한 개인 경우 origin을 사용함.
git remote -v => repository 확인

8) 원격 저장소 삭제
git remote rm <이름>
git remote remove <이름>

9) 원격 저장소에 업로드
git push <저장소 이름><브렌치 이름>