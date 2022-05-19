<p align="center">
라이트웨이 리눅스에 관해 궁금한 점이 있거나 사용 중 도움이 필요하십니까?
</p>

<h2 align="center">설치하기</h2>

1. BIOS 설정에 진입하여 Secure Boot를 비활성화하십시오. 메인보드 제조사, PC 제조사마다 진입 키가 다릅니다.
2. 설치 미디어가 장착되었으면 부팅 메뉴를 불러오십시오. 부팅 메뉴 키는 F9, Del 등 제조사마다 다릅니다.
3. 바탕화면 및 독에 위치한 칼라마레스 아이콘을 클릭하십시오.

<h3 align="center">Windows와 함께 설치</h3>

새로운 컴퓨터에서 설치하실 땐 반드시 Windows를 먼저 설치하신 후 파티션을 조정하고 lightway를 설치하셔야 합니다.

<h3 align="center">ChromeOS 듀얼부팅</h3>

brunch framework의 페이지를 참고하십시오. 

<p align="center">(* ChromeOS와 듀얼부팅은 Secure Boot와 같이 사용하실 수 없습니다.)</p>

<h2 align="center">운영체제 사용</h2>

<h3 align="center">데스크탑 환경</h3>

라이트웨이는 KDE Plasma, 그놈, Xfce 에디션을 제공하며, 각 에디션별 UI 구성은 데스크탑 환경의 기본 UI를 따릅니다.

KDE Plasma와 그놈은 데스크탑 환경 차원에서 도움말을 제공합니다.

<h3 align="center">모바일 연동</h3>

KDE Plasma 에디션은 KDE Connect가 선탑재되어 설치 즉시 스마트폰과 연동하실 수 있으며, 그놈 에디션은 GSConnect를 설치하신 후 로그아웃하고 다시 로그인하거나 Xorg에선 Alt + F2 키를 누르고 r을 입력하시면 확장을 활성화하실 수 있습니다.

KDE Connect 앱은 안드로이드 스마트폰, iPhone에서 사용하실 수 있습니다.

<p align="center">(* Xfce 에디션에서는 공식적으로 작동을 보장하지 않습니다.)</p>

<h3 align="center">프로그램 설치</h3>

아치 리눅스는 pacman을 패키지 관리자로 사용하며, 패키지 파일은 pkg.tar.zst 형식입니다.

또한, 아치 리눅스 저장소에서 제공하지 않는 패키지는 AUR Helper를 통해 설치할 수 있습니다. yay를 AUR 헬퍼로 제공할 예정입니다.

```
sudo pacman -S           < 프로그램 설치 >
sudo pacman -Rcn         < 프로그램과 필수 의존성 삭제 >
sudo pacman -Rnn         < 프로그램 삭제 >
sudo pacman -Rdd         < 의존성을 무시하고 프로그램 삭제 - 시스템에 문제를 일으킬 수 있으므로 권장하지 않습니다. >
sudo pacman -U           < 패키지 파일 설치 >
```

<h4 align="center">다른 패키지 관리자 사용</h4>

라이트웨이는 flatpak을 선탑재하고 있으며, flatpak install으로 프로그램을 설치하실 수 있습니다. 또한, 우분투의 패키지 관리자인 snap을 AUR에서 설치하실 수 있습니다.

<h3 align="center">시스템 업데이트</h3>

사용자 경험과 보안 향상을 위해 되도록이면 소프트웨어를 최신 버전으로 유지해야 합니다. 

<h4 align="center">명령줄 도구 사용</h4>

1. 데스크탑 환경에서 제공하는 터미널(그놈 터미널, Konsole, Xfce 터미널 등)을 실행하십시오.
2. 컴퓨터가 인터넷에 연결되어 있는지 확인한 후 sudo pacman -Syu를 입력하십시오.
3. 패키지가 설치될 때까지 터미널 창을 닫지 말고 기다리세요.
4. 업데이트가 완료되었으면 터미널을 닫으십시오. 다만, 커널과 데스크탑 환경 등 중요 업데이트가 이루어졌을 경우 하던 작업을 모두 저장하신 후 컴퓨터를 다시 시작하십시오.

<h4 align="center">GUI</h4>

GUI 패키지 관리 도구는 그놈 소프트웨어, Discover 등 데스크탑 환경의 구성요소로 제공되며, Xfce는 AUR을 통해 pamac을 설치하셔야 합니다.
