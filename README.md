1)리눅스 명령어(top, ps, jobs, kill)
---
#### 1) top : 시스템 프로세스/ 메모리 사용 현황을 실시간으로 출력한다.

* top –d 갱신시간 : 화면 갱신시간을 설정한다.

* top –q : 화면을 계속 갱신한다.

* top –i : idle 상태와 zombie 프로세스를 무시한다.
---
#### 2) ps : 현재 실행중인 프로세스를 보여주는 리눅스 명령어이다. 현재 프로세스들의 상태를 PID(Process ID)와 함께 보여준다. 리눅스에서는 사용자와 파일 뿐만 아니라 프로세스 번호로 관리한다.
 
* ps -a : 다른 사용자에 의해서 생성된 프로세스들도 보여준다.
 
* ps -u : 프로세스의 소유자에 대한 정보 등 매우 자세하게 보여준다.
 
* ps -l : 프로세스의 정보를 옆으로 길게 보여준다.
 
* ps -x : daemon process등 터미널의 컨트롤과 관련이 없는 프로세스도 보여준다. 일반적으로 말하는 데몬프로세스도 보여준다. 
 
* ps -e : 해당 프로세스에 관련된 환경변수 정보를 함께 출력한다.

* ps –f : 프로세스 간의 상속관계를 보여준다.
---
#### 3) jobs : 작업이 중지된 상태나 백그라운드로 진행 중인 상태를 표시

* jobs –l : 프로세스 번호를 추가해서 보여준다.
---
#### 4) kill : 프로세스에 특정한 시그널을 보내는 명령이다. 보통 실행중인 프로세스에 종료 신호를 보낸다. 보통 중지시킬 수 없는 프로세스를 종료시킬 때 많이 사용한다. 

* kill –l [-시그널 번호 또는 –시그널이름] % 작업번호 : 시그널의 종류(시그널 번호 순서대로)를 나열한다. 
---
2.vim에디터에서 매크로 사용법
