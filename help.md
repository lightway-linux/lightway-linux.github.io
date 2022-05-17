<p align="center">
라이트웨이 리눅스에 관해 궁금한 점이 있거나 사용 중 도움이 필요하십니까?
</p>

<h2 align="center">설치하기</h2>

<h2 align="center">운영체제 사용</h2>

<h3 align="center">데스크탑 환경</h3>

KDE Plasma와 그놈은 데스크탑 환경 차원에서 도움말을 제공합니다.

<h3 align="center">프로그램 설치</h3>

아치 리눅스는 pacman을 패키지 관리자로 사용하며, 패키지 파일은 pkg.tar.zst 형식입니다.

또한, 아치 리눅스 저장소에서 제공하지 않는 패키지는 AUR Helper를 통해 

 sudo pacman -S           < 프로그램 설치 >
 sudo pacman -Rcn         < 프로그램과 필수 의존성 삭제 >
 sudo pacman -Rnn         < 프로그램 삭제 >
 sudo pacman -Rdd         < 의존성을 무시하고 프로그램 삭제 - 시스템에 문제를 일으킬 수 있으므로 권장하지 않습니다. >
 sudo pacman -U           < 패키지 파일 설치 >

<h3 align="center">시스템 업데이트</h3>

사용자 경험과 보안 향상을 위해 되도록이면 소프트웨어를 최신 버전으로 유지해야 합니다. 

<h4 align="center">명령줄 도구 사용</h4>

1. 데스크탑 환경에서 제공하는 터미널(그놈 터미널, Konsole, Xfce 터미널 등)을 실행하십시오.
2. 컴퓨터가 인터넷에 연결되어 있는지 확인한 후 sudo pacman -Syu를 입력하십시오.
3. 패키지가 설치될 때까지 터미널 창을 닫지 말고 기다리세요.
4. 업데이트가 완료되었으면 터미널을 닫으십시오. 다만, 커널과 데스크탑 환경 등 중요 업데이트가 이루어졌을 경우 하던 작업을 모두 저장하신 후 컴퓨터를 다시 시작하십시오.

<h4 align="center">GUI</h4>

GUI 패키지 관리 도구는 그놈 소프트웨어, Discover 등 데스크탑 환경의 구성요소로 제공되며, Xfce는 AUR을 통해 pamac을 설치하셔야 합니다.
