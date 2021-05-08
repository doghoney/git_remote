# __readme 개요__

## __시나리오__
- 프로젝트를 git으로 관리하기 시작
  1. 현재 문서의 상태 : x
  2. 바꾸고 싶은 상태 : x
  3. 목적 : .git이라는 하위 디렉토리 생성
  4. 사용하는 법: $git init


- 파일을 stage
  1. 현재 문서의 상태 : modified
  2. 바꾸고 싶은 상태 : staged
  3. 목적 : 해당 파일을 commit하려는 스냅샷으로 추가한다.
  4. 사용하는 법: $git add \<filename>


- 앞으로 사용할 단축 명령어를 생성
  1. 현재 문서의 상태 : x
  2. 바꾸고 싶은 상태 : x
  3. 목적 : 단축된 git 명령어(or 별칭) 사용
  4. 사용하는 법: $git config --global alias.ci commit


- staged 된 스냅샷을 저장소에 저장
  1. 현재 문서의 상태 : staged
  2. 바꾸고 싶은 상태 : commmitted
  3. 목적 : staging area에 담긴 내용을 commit
  4. 사용하는 법: $git commit
  5. 주요 옵션 : <br>
    [-a] : tracked 상태의 파일을 자동으로 Stgaing Area에 넣는다.<br><br>

- Modified된 파일 되돌리기
  1. 현재 문서의 상태 : Modified
  2. 바꾸고 싶은 상태 : Unmodified (이전 commit 상태)
  3. 목적 : 현재 수정중인 문서를 버리고 이전으로 돌아감
  4. 사용하는 법: $git checkout -- \<filename> <br><br>

- working directory 업데이트
  1. 바꾸고 싶은 상태 : 이전 commit으로 working directory 변경
  2. 목적 : working directory를 이전 commit으로 초기화
  3. 사용하는 법: $git reset --hard \<sha1> <br><br>

- 현재 파일의 수정 및 staged 여부 확인
  1. 현재 문서의 상태 : x
  2. 바꾸고 싶은 상태 : x
  3. 목적 : 현재 파일이 이전 commit과 비교해 수정 및 staged 여부를 확인한다.
  4. 사용하는 법: $git status
  5. 주요 옵션 : <br>
    [-s],[--short] : 간단한 변경내용만을 보여준다. <br><br>

- tag 달기
  1. 현재 문서의 상태 : untagged
  2. 바꾸고 싶은 상태 : tagged
  3. 목적 : tag 달기
  4. 사용하는 법: $ git tag \<tagname>
  5. 주요 옵션 : <br>
    [-a] : Annotated 태그 생성 <br>
    [-m "\<message>"] : 메시지도 저장 <br><br>

- tag 확인
  1. 현재 문서의 상태 : tagged
  2. 목적 : tag 확인
  3. 사용하는 법: $git tag    <br><br>
- tag로 checkout
  1. 현재 문서의 상태 : tagged
  2. 목적 : tag를 통해 checkout
  3. 사용하는 법 : $git checkout \<tag>  <br><br>

- commit history 조회
  1. 현재 문서의 상태 : committed 여러
  2. 목적 : commit history를 시간순으로 조회
  3. 사용하는 법: $git log
  4. 주요 옵션 : <br>
    [-p] : 각 커밋의 diff 결과를 보여준다. <br>
    [-2] : 최근 두 개의 결과만 보여준다.   <br>
    [-stat] : history의 통계를 보여준다.  <br>
    [--pretty=oneline] : 각 commit당 한 라인  <br><br>

- branch 생성
  1. 현재 문서의 상태 : master branch에서 작업 진행중
  2. 바꾸고 싶은 상태 : master branch에서 새로운 branch 뻗기
  3. 목적 : 작업중이던 마지막 commit에 새로운 branch 생성
  4. 사용하는 법: $git branch \<branchname>
  5. 주요 옵션 : <br><br>

- branch 삭제
  1. 현재 문서의 상태 : branch A에서 작업 진행중
  2. 바꾸고 싶은 상태 : branch B삭제
  3. 목적 : branch 삭제
  4. 사용하는 법: $git branch -d \<branchname : B>


- branch 이동
  1. 현재 문서의 상태 : branch A에서 작업 진행중
  2. 바꾸고 싶은 상태 : branch B에서 작업 진행
  3. 목적 : 다른 branch로 이동
  4. 사용하는 법: $git checkout \<branchname : B> <br><br>

- branch 병합
  1. 현재 문서의 상태 : branch A에서 작업 진행중
  2. 바꾸고 싶은 상태 : branch B를 branch A에 병합 후 진행
  3. 목적 : branch B를 현재 branch에 병합
  4. 사용하는 법: $git merge \<branchname : B> <br><br>

- 원격 저장소에서 git 저장소 불러오기
  1. 현재 문서의 상태 : x
  2. 바꾸고 싶은 상태 : 프로젝트 생성
  3. 목적 : 해당 url로부터 git 저장소 복사
  4. 사용하는 법: $git clone \<url>
  5. 주요 옵션 : <br>
    $git clone <url> \<changed name> : 디렉토리 이름을 changed name으로 바꿈 <br><br>

- remote 저장소 확인하기
  1. 현재 문서의 상태 : 프로젝트에 리모트 저장소가 등록되있음
  2. 목적 : 현재 프로젝트의 리모트 저장소 확인
  3. 사용하는 법: $git remote
  4. 주요 옵션 : <br>
    [-v] : 단축이름(이하 remote)과 URL 함께보기 <br><br>

- remote 저장소 추가하기
  1. 목적 : 기존 working directory에 새 remote 저장소 추가
  2. 사용하는 법: $git remote add \<remote> \<URL> <br><br>

- 로컬 branch를 원격 저장소에 올리기
  1. 현재 문서의 상태 :
  2. 바꾸고 싶은 상태 :
  3. 목적 : 로컬 저장소에 만들어 놓은 branch를 원격 저장소에 올린다.
  4. 사용하는 법: $git push \<remote> \<branch name>
  5. 주요 옵션 : <br>
    $git push <remote> [--all] : 모든 브랜치 전송 <br><br>

- 원격 저장소에서 불러오기
  1. 현재 문서의 상태 : 원격저장소에 있지만 문서에 없는 내용 존재
  2. 바꾸고 싶은 상태 : 없는 내용 불러오기 + merge
  3. 목적 : 원격에 있지만 로컬에 없는 내용을 불러와서 merge 한다.
  4. 사용하는 법: $git pull \<remote> \<branch name> <br><br>

- branch 통일
  1. 현재 문서의 상태 : branch A와 branch B 두갈래로 나뉨
  2. 바꾸고 싶은 상태 : branch A 변경사항을 branch B쪽에  적용
  3. 목적 : branch를 하나로 통일시킨다.
  4. 사용하는 법: <br>
    $git checkout \<branchname : B>
    $git rebase \<branch name : A>
