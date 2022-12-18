# Raspberry PI 4 Multiple Object Tracking(수정중)
## Client  

### ※ 필요 Library : OpenCV, Cmake  

### ※ 사용 언어 : C/C++  

### ※ Raspberry PI 4 구동환경에서 구현되었으며, 다른 버전에서는 구동되지 않습니다  
(다른 버전에서는 I/O Peripheral 시작 주소 및 오실레이터 주파수 변경이 필요)  
  
  
클라이언트 프로그램에서는 크게 두가지 기능을 수행합니다.
<br>첫번째로 영상을 실시간으로 촬영하고, 이를 UDP 소켓을 통해 서버로 전송하는 기능입니다.
<br>빠른 영상 전송을 위해 영상의 크기는 320x240 크기로 고정시켰으며, 이는 설정파일을 통해
<br>사용자가 직접 변경할 수 있습니다.<br>
<br>두번째로 UDP 소켓에서 명령어를 전달받아 기기의 모터 및 센서를 제어하는 기능입니다.
<br>라즈베리파이 기기에서는 디바이스 드라이버를 통해 외부 라이브러리 사용하지 않고 구현하였으며,
<br>


### 전체적인 구동
