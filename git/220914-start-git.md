# git 사용법

## git 명령어
- git에서 사용하는 기본적인 명령어들을 배웠다
1. cd : 디렉토리 이동
2. mkdir : 현재 디렉토리에 폴더 생성
3. rm, rm -r ; 디렉토리나 파일을 삭제할 때 rm, 비어있지 않다면 rm -r
4. cp : cp [옵션][복사 할 디렉토리/파일][복사 될 디렉토리/파일]
5. vi : 파일내용 수정
6. mv : mv (옵션) (이동할 파일 이름) (이동시킬 위치)
7. cat : 해당 하는 파일내용을 간단하게 출력
8. ls : 현재 폴더에 있는 파일 목록 출력
git add, git commit, git push, git status 

## vi 명령어
1. :q : 종료 (저장x)
2. :q! : 강제 종료(저장x)
3. :w : 저장
4. :wq : 저장하고 종료
5. i : 내용을 정할 수 있는 Insert mode
6. ESC : Insert mode에서 normal mode로 돌아감

## branch
1. git branch 브랜치이름 : 해당 이름의 branch 생성
2. git switch 브랜치이름 : 해당 브랜치로 이동
3. git branch -D 브랜치이름 : 브랜치 삭제
4. git merge 브랜치이름 : 해당 브랜치를 가져와서 현재의 branch에 병합
5. merge conflict : 동시에 같은 줄의 내용에 변화가 있을 때 발생
6. git remote add remote이름 remote주소 : remote의 이름변경
