sumo 사용법 익히기!

https://eclipse.dev/sumo/
위 링크에서 간편하게 windows용 sumo 다운 가능(리눅스 환경 X)

https://sumo.dlr.de/docs/Tutorials/index.html
위 링크의 여러 튜토리얼 중 Hello World와 OSMWebWizard를 따라해봤다.

1. https://sumo.dlr.de/docs/Tutorials/Hello_World.html
위 튜토리얼에서 기본적인 sumo의 개념과 작동방식을 알았다.
sumo 다운로드시 함께 다운로드 된 netedit에서 실행시킬 네트워크, 교통 개체를 만들어준다.
그 후 .sumocfg 확장자의 파일로 전체 네트워크를 저장한 후 sumo를 이용해 실행시켜준다
이때 permision 어쩌고 하면서 다운이 안될 수 있는데 그럼 C:\Program Files (x86)\Eclipse 경로의
Sumo 폴더를 우클릭, 속성, 보안, 편집, 위쪽 창 그룹 또는 사용자 이름에서 User(어쩌고저쩌고)를 클릭 후
아래쪽에 모든 권한, 적용을 클릭하면 sumo 파일에 관리자 권한을 부여하게 된다.
다시 netedit에서 sumocfg파일 저장을 해보면 잘 될것이다.

2. https://sumo.dlr.de/docs/Tutorials/OSMWebWizard.html
osmWebWizard를 사용해 세계지도에서 원하는 부분을 sumo에서 시뮬레이션 할 수 있다.

cmd를 켜준다.
cd .. 명령어로 C:\ 디렉토리로 이동한다.

그 후 cd C:\Program Files (x86)\Eclipse\Sumo\tools
를 입력해 해당 디렉토리로 이동 후
python osmWebWizard.py를 입력해 osmWebWizard를 실행해준다.
(python 2.7이상이 깔려있어야한다.)

오른쪽 position에서 "36.634901 127.460026" 를 입력하면 사창사거리로 간다.
사창사거리 좌표이다.

오른쪽 사이드에 vehicles(자동차모양) 클릭하여 시뮬레이션하고싶은 운송수단을 선택해야한다.
사창사거리에 Trams, Urban trains, Trains, Ships는 나올 일 없으므로 체크해제한다.
만약 체크하면 sumo가 해당 파일 못찾았다면서 오류를 발생시킨다.

이제 Generate Scenario해주고 시뮬레이션 해준다.

![image](https://github.com/DoHyung08/RL/assets/73733984/5a832778-7a64-4e1e-a9b2-c7a472eaa5cf)

