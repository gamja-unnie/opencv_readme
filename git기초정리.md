# <span style = "color: pink">**git 기초**</span>

##  git 초기설정
: 최초 한 번만 설정<br>
1. 누가 커밋 기록을 남겼는지 확인할 수 있도록 이름과 이메일 설정
    * git config --global user.name "이름" 
    * git config --global user.email "이메일 주소"
2. 작성자가 올바르게 설정되었는지 확인
    * git config --global -list

 -------------------
 <br>

## git 기본 명령어
1. 로컬 저장소
    * Working Directory : 사용자의 일반적인 작업이 일어남
    * Staging Area : 커밋을 위한 파일 및 폴더가 추가되는 곳
    * Repository : staging area에 있던 파일 및 폴더의 변경사항을 저장하는 곳
    * Working Directory-> Staging Area -> Repository
2. ***git init***
    * 현재 작업중인 디렉토리를 Git으로 관리한다는 명령어
    * `.git` 이라는 숨김 폴더를 생성하고, 터미널에는 `(master)`라고 표기됨
3. ***git status*** 
    * Working Directory와 Staging Area에 있는 파일의 현재 상태를 알려줌
    * 상태 
        - Untracked : Git이 관리하지 않는 파일 (한 번도 Staging Area에 올라간 적 없는 파일)
        - Tracked : Git이 관리하는 파일 
            * unmodified: 최신상태
            * modified : 수정되었지만 아직 staging area에 반영x
            * staged : staging area에 올라간 상태
4. ***git add***
    * Working Directory에 있는 파일을 Staging Area로 올리는 명령어 
    * Staged상태가 되도록 함
5. ***git commit***
    * Staging area에 올라온 파일의 변경 사항을 하나의 커밋으로 저장
6. ***git log***
    * 커밋의 내역을 조회
    * `--one line` : 한 줄로 축약<br> 
     `--graph` : 그래프로 <br>
      `--all` : 모든 내역<br>
       `--reverse` : 반대로 <br> `-p` : 변경 내용도 같이 <br> `-숫자` : 원하는 갯수만큼 


