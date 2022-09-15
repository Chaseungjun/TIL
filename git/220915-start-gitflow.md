## git Bash로 진행하는 깃 플로우 순서
1. git flow init : develop branch 생성됨
2. git branch 로 확인
3. git flow feature start (설정할 feature이름) : feature branch를 생성하면서 자동으로 feature branch로 이동
4. feature 파일이 완성되면 커밋 (한 번에 완성하지말고 의미있는 완성 단위를 나누어서 add, commit)
5. feature를 모두 완성하면 git flow feature finish (feature이름)  -> Merge commit가 나오는데 내용은 안적어도 됨 , 
feature를 종료하면서 develop으로 merge 그리고 develop branch로 자동으로 이동, feature는 자동삭제
6. git flow release start (버전name)
7. git flow release finish (버전name) -> main과 develop에 하나씩 넘겨주게됨
main branch에 대한 merge commit, merge된 commit에 대해 tagging 하는 commit(release 노트작성), develop에 들어가는 commit
8. git push -u origin develop : 로컬에는 develop 이 있지만 원격저장소에는 없는 상황에 develop branch를 알려줌 (-u는 이름뿐만아니라 내용까지 같음을 알려주는데 처음 알려줄때만 쓰고 이후엔 사용하지 않아도 됨)
9. git switch main
10 git push origin main
=> git push는 release가 끝나고 develop과 main에서 각 한 번씩 해주면 됨
11. git push --tags
12. git switch develop - git flow frature start 하면서 다시 시작
