# Dockerfile

- FROM: Base이미지(OS이미지 등)로 사용할 Layer를 가져오는 단계
- LABEL: Meta 정보를 입력하는 부분(빌드 자동화 등에 사용, 기능동작x)
- RUN: 설치/설정 등을 위한 실행 부분(수행해야하는 커맨드)
- ENV: 환경변수에 대한 선언
- COPY: Local 디스크의 파일을 컨테이너 내부로 복사
- ENTRYPOINT: 런타임시에 최종적으로 실행 되는 명령어
- EXPOSE: Port를 외부로 mapping 하기 위한 정보
