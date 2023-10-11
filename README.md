# TIL-test-

TIL 을 새로 작성 하려는데, 이전 프로젝트(팀 자스민)에서 작업 초반 Branch 때문에 애를 먹었던 게 생각났다.
VScode에서 작성을 하고 Push, Pull 연습도 겸하는 도중 git init 을 하니 자동으로 Branch가 Main으로 생성된다는 걸 알게 되었다.
이걸 어떻게 바꾸나?

공대돌고래(https://donghunee.github.io/study/2021/03/17/git/) 에서 보니 git config –global init.defaultBranch main 라고 터미널에 입력해 주면 된다고 한다.
그 결과
$ git config –global init.defaultBranch main~
error: key does not contain a section: –global
라고 에러 메세지가 뜬다.

사실 위 에러 메세지가 왜 뜨는지는 안알아봤고 팀원의 도움을 받았는데,
깃허브 repository 세팅에서 branch의 default값을 main으로 바꾼 후 Update 하였고, 
깃허브에서 만들어놓은 repository : TIL-test2-(연습용) 를 VSCode로 clone 하니 branch값이 'master'에서 깃허브에서 설정해 놓은 ''