# ROS2--1-2

1. 윈도우 ipconfig 실행 및 결과 설명

실행 방법
Win + R 키를 누르고 cmd를 입력하여 명령 프롬프트(터미널)를 엽니다.
ipconfig (또는 자세한 정보를 위해 ipconfig /all)를 입력하고 Enter를 누릅니다.

주요 출력 항목 설명
IPv4 주소 (IPv4 Address): 내 PC가 현재 네트워크(공유기 등)에서 할당받은 유일한 내부 IP 주소입니다.
서브넷 마스크 (Subnet Mask): IP 주소 중 어디까지가 네트워크 영역이고 어디까지가 개별 PC(호스트) 영역인지 구분해 주는 값입니다.
기본 게이트웨이 (Default Gateway): 외부 인터넷 망으로 나가는 통로가 되는 장비(주로 공유기/라우터)의 IP 주소입니다.



2. 리눅스(WSL) ifconfig 실행 및 결과 설명

실행 방법
Ubuntu 터미널을 엽니다.
ifconfig를 입력합니다.
(만약 명령어가 없다고 나오면 sudo apt update && sudo apt install net-tools 명령어로 설치 후 실행합니다.)

주요 출력 항목 설명
eth0 (또는 enp0s3 등): 실제 또는 가상 네트워크 카드 인터페이스입니다.
inet: 해당 리눅스 서버가 할당받은 IPv4 주소입니다. (WSL 원격 접속 시 이 IP 주소를 사용합니다.)
netmask / broadcast: 서브넷 마스크 및 브로드캐스트 주소 정보입니다.
RX / TX packets: 네트워크로 수신(RX) 및 송신(TX)한 데이터 패킷의 양과 에러 수입니다.
lo (Loopback): 자기 자신(Localhost, 127.0.0.1)을 가리키는 내부 테스트용 가상 네트워크 인터페이스입니다.
