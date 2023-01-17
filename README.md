# Git hub 사용법

#Git

                git init 은 절대 홈디렉토리에서 사용 금지
  
1. 기능 

  - ls
  - cd TIL/          폴더 들어가기

  - touch a.txt   / 폴더에 a 텍스트 만들기
  - touch a.txt b.txt c.txt   / 여러개
  - touch README.md

  - vim a.txt        / 텍스트 들어가기
  - :q                / 나가기
  - rm a.txt         / 텍스트 삭제
  - rm -r day02    / day02 폴더 삭제

  - start .           / 현재 폴더를 띄워줌
  - code .          / 현재 폴더의 vscode를 실행시켜줌



2. 매커니즘 

  - working directory 작업공간

  - staging area 특정파일이 있는곳

  - Repository 커밋들 저장되는곳

3. git 이용법

 - git init         저장소 생성
 - touch README.md       파일 생성
 - git add README.md       올리기 ( or . 가능)
 - git status                                 (상태확인)
 - git config --global user.name "Joungwon"
 - git config --global user.email "15gpfk@naver.com"
 - git commit -m 'first commit'        저장소에 저장

4. 변경
 - git branch -M main          (or master) 


5. 사이트 연동
 - git remote add origin https://github.com/Joungwon/Note.git


6. 파일 올리기
 - git push origin master          


8. 
- 파일 수정 :


- 파일 만들기 :
  -  touch a.txt b.txt c.txt
  -  git add .
  -  git commit -m 'txt file'
  -  git push -u origin main    인터넷에 업로드


- 파일 삭제 :
  -  rm b.txt c.txt
  -  git add .
  -  git commit -m 'txt file'
  -  git push -u origin main



9. 복사 기능  git clone https://github.com/Joungwon/Note.git



10. 
- git hub에 저장소 생성
    - git remote add origin {저장소주소}
- 원격저장소에 push
    - git push -u origin master




11. 원격저장소에서 --> 강의실컴으로

- 강의실에서
  - git clone {주소} .      // 불러오기
  - 수정
  - git add .
  - git commit -m'daf'
  - git push

- 집에서
  - git pull origin main            // master  or main



# 파일 공유
- git pull -> 수정 -> git add -> git commit -> git push

# gitignore 사이트  
- touch README.md .gitignore     숨김파일 생성
- gitignore 사이트에서 충돌파일 복사 -> .gitignore 파일에 복사
-  ``` add 하기전에 



# github기능  :  Markdown 마크다운 

기능) heading

  #: 제목앞에
  - : 소주제
  1. : 숫자

  `a` : 코드 강조

  ``` : 코드 강조2
  ```

  [strint](url)  : 링크 기능

  [다른 파일](../afolder/other.md)   : 다른 파일로 넘어가는 기능

  ![strint](img_url)   : 이미지 링크 기능
 
  기울임
