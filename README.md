top 명령어

Linux 프로세스를 표시하는데 사용된다.

실행중인 프로세스를 실시간으로 보는 것을 제공해 준다.

일반적으로 이 명령어는 시스템의 요약 정보와 현재 리눅스 커널에서 관리하는 프로세스 또는 쓰레드 목록을 보여준다.

이 명령을 실행 하면 위쪽 절반에 프로세스 및 리소르 사용 통계가 포함되는 명령어 모드가 열린다.

하단에는 현재 실행중인 프로세스 목록이 포함 되어 있다. q를 누르면 명령 모드가 종료한다.

보여주는 목록들로는 PID, PR, VIRT, CPU, TIME, SHR, NI, MEM, RES, COMMAND

PID : 작업의 고유 프로세스 ID를 표기한다.
PR : 프로세스의 우선순위를 나타낸다. 숫자가 낮을수록 우선순위가 높다.
VIRT : 작업에서 사용한 총 가상 메모리이다.
USER : 작업 소유자의 사용자 이름이다.
CPU : CPU사용량을 나타낸다.
TIME :  CPU 시간, TIME과 동일 하지만 100분의 1초를 통해 더 세분화 하여 나타낸다.
SHR : 작업에서 사용하는 공유 메모리 크기(kb)를 나타낸다.
NI : 작업의 좋은 가치를 나타낸다. nice 값이 음수이면 우선순위가 높고 nice값이 양수이면 우선순위가 낮다.
MEM : 작업의 메모리 사용량을 보여준다.
RES :  프로세스가 사용중인 물리적 RAM의 양(kb)이다.
COMMAND : 프로세스를 시작한 명령의 이름.

옵션

ex 1) top -n 10
특정 반복 후 상단 명령 종료 : top 출력은 'q'를 누를 때 까지 계속 새로고침 된다. top -n 10을 사용하면 top명령은 총 10번 반복 후에 자동으로 종료 된다.

ex 2) top -u paras
특정 사용자 프로세스를 표시 하여 준다.

ex 3) top -h
상단에서 실행중인 프로세스를 강조하여 표시해 준다. 실행중인 상단 명령에서 'z'옵션을 누르면 실행중인 프로세스를 색상으로 표시하여 쉽게 실행중인 프로세스를 식별하는 데 도움이된다.

ex 4) top -b
배치 모드 : 상단에서 파일이나 다른 프로그램으로 출력을 보낸다.

ex 5) top -s
보안 모드 : 보안 모드에서 top명령을 사용한다.

ex 6) top -c
명령줄 : 마지막으로 닫힌 상태로 맨 위에서 시작한다.

ex 7) top -d seconds.tenths
delay(지연시간) : 화면 업데이트 사이의 지연 시간을 알려준다.
