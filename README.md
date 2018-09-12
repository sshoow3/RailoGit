# RailoGit

2018.09.12 

이클립스 Git Hub 연동 test
업로드시 수정한점

1. .gitignore 설정파일 추가
Eclipse Project의 모든 파일이 업로드 되는것이 아닌
import에 필요한 데이터만 업로드하도록 제한

2. Project의 설정 수정쟈
windows - preferences - Maven - Java EE Integration
에서 Maven Archiver generates files under the build directory 체크해제

------------------------------------------------------------------
git 연동 순서

1. 원격저장소 와 Git Repositories 로컬저장소 연동
프로젝트와 Git Repositories 연결

Git Repositories의 Directory에 있는 Project에 .gitignore 생성

.gitignore 설정 방법은 구글 검색하면 많이 나온다.

Working Directory - (Project) 에 위치해 있는 .gitignore 

add index 후 commit and push

.gitignore 가 원격저장소에 올라갔는지 확인 후 제대로 올라갔다면 

project 를 addindex 하고 commit and push 하면 된다.
------------------------------------------------------------------
import 
.gitignore 에서 .project , .classpath 와 같은 프로젝트구성요소가 부족하기 때문에
추가 작업이 필요하다.

import - Git - Projects from Git - Clone URI
로 원격저장소의 프로젝트에 접근하여
프로젝트를 선택한다.

그후  - Select a wizard to use for importing projects 에서는 

Import as general project를 선택하는데

Working Directory 에 바로 프로젝트가 잇는경우와
Working Directory 안에 폴더로 프로젝트가 있는경우가 있는데

아래의 경우 바로 호출하기 때문인지 비어있는것으로 보일때가 있어
Back으로 뒤로갔다 다시 Next로 오면 프로젝트가 보인다.

Working Directory - (Project) 클릭 후 Next Project 이름을 입력하고 final 을 클릭시

위에 말하였다 싶이 구성요소가 부족해 현재 그냥 Project 혹은 Java Project 상태이다.

Import한 Project를 마우스 우측버튼 클릭 후 
Configure - Convert to Facted From 클릭 후 

프로젝트 에 맟춰 사양 번경 하거나 그냥 나오면 된다.

그후 
Configure - Convert to Maven Project 를 클릭하면 

정상적으로 MVC 패턴 동작하는것을 확인하였다.



위처럼 복잡한 방법이 아닌 간편한 방법이 있을 수 있겠지만
위의 내용은 필자가 혼자서 여러가지 검색해보며

처음으로 작동 성공한 것으로 기록해 둔 것이다.

이후에도 이것저것 시도해가면서 더 간편하고 간단한 연동과 Import 방식을 찾을것이다.
