1)리눅스 명령어(top, ps, jobs, kill)
---
#### 1) top : 시스템 프로세스/ 메모리 사용 현황을 실시간으로 출력한다.
<ima src ="https://user-images.githubusercontent.com/106420653/171998514-5e5bcadb-dfaa-4de0-ad45-476dd91f6d4e.png" width="600" height="400">

* top –d 갱신시간 : 화면 갱신시간을 설정한다.

* top –q : 화면을 계속 갱신한다.

* top -c : command list 전체를 보여준다.

* top –i : idle 상태와 zombie 프로세스를 무시한다.
---
#### 2) ps : 현재 실행중인 프로세스를 보여주는 리눅스 명령어. 현재 프로세스들의 상태를 PID와 함께 보여주며, 리눅스에서는 사용자와 파일 뿐만 아니라 프로세스도 번호로 관리한다.
![image](https://user-images.githubusercontent.com/106420653/171998374-ff73ad6a-285a-47a5-9bd7-d809eb1109e0.png)

* ps -ef : 모든 프로세스를 풀 포맷으로 출력한다.

* ps a : 현재 터미널의 사용자 고유 프로세스를 출력한다.
 
* ps u : 프로세스의 소유자의 이름, CPU 사용량, 메모리 사용량 등 상세 정보를 출력한다.
 
* ps -e : 커널 프로세스를 제외한 모든 프로세스를 출력한다.
 
* ps -u [사용자이름] : 특정 사용자에 대한 모든 프로세스의 정보를 출력한다.
---
#### 3) jobs : 백그라운드로 실행중인 프로세스나 현재 중지된 프로세스의 목록을 출력해주는 명령어이다.

![image](https://user-images.githubusercontent.com/106420653/171998424-b017c446-e2ba-4e93-8446-b58a93278613.png)

* jobs –l : 프로세스 번호를 추가해서 보여준다.
---
#### 4) kill : 실행중인 프로세스에 특정한 시그널(종료 신호)를 보낸다. 보통 중지시킬 수 없는 프로세스를 종료시킬 때 많이 사용한다. 
<img sre="https://user-images.githubusercontent.com/106420653/171998583-59e5932e-04ff-41b1-9dc0-0d19f9cde2ac.png" width="600" height="400">

* kill –l : 시그널 리스트를 나열한다. 시그널 번호와 시그널 이름은 매치되어서 보여줌.

* kill -s : 특별히 보낼 시그널을 지정함. 시그널 번호나 시그널 이름을 지정함.

* kill -9 PID : 강제종료
 
* kill -HUP PID : 종료된 프로세스를 다시 되살림.

> PID: 프로세스 ID 
---
---
2.vim에디터에서 매크로 사용법
---
먼저 매크로를 실행하는 방법은 명령모드에서 q[name]을 해준다.

그 다음 반복해서 실행할 행동을 매크로 입력해준다.

q를 입력해서 매크로를 종료한다.

마지막으로, 등록된 매크로를 실행시키는 방법은 @[name]을 해준다.

이때 @[name] 앞에 [숫자]@[name]을 하게 되면 숫자의 횟수만큼 매크로를 실행하게 된다.
