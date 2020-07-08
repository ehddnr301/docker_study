# Docker 🚀

## 사용이유 ?

- 컨테이너에 미리 담아서 배포할때 컨테이너를 올려 배포진행이 편하게 합니다.

## 특징

- 컨테이너는 도커 엔진 위에서 동작
- 서버를 업데이트 할때는 새로운 도커이미지를 업데이트해서 컨테이너에 올리고 기존의 컨테이너는 제거합니다.

## 구성

- Docker Engine : 특정 소프트웨어를 도커 컨테이너로 만들고 실행하게 해주는 데몬을 의미합니다. 도커 엔진과 도커 클라이언트 사이에는 REST API가 사용됩니다. REST API 서버에 요청을 보내는 것이 Docker Client 입니다.

- Docker Client : 도커 엔진과 통신하는 소프트웨어로 개발자가 직접 이용할 수 있습니다. 윈도우/맥/리눅스 를 지원합니다.

- Docker Host OS : 도커 엔진을 설치할 수 있는 운영체제 환경을 의미합니다.

## 설치

- Docker For Mac과 Docker Toolbox의 차이점은?
  - 가장 큰 차이점은 사용하는 가상머신이 다르다는 점입니다. Docker Toolbox 같은 경우에는 Boot2Docker에서 사용해왔던 VirtualBox를 그대로 사용합니다. 
  - 반면에 Docker for Mac은 HyperKit 이라는 macOS를 위한 경량화 가상머신을 사용합니다.