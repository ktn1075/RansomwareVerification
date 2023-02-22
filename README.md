# RansomwareVerification
- 개요 : 실제 렌섬웨어와 치료 도구를 가상 OS에 전송하여 감염 시키고 치료 도구의 유효성을 확인한다.
</br> 가상OS 내의 설치되는 Agent와  Agent 들을 관리하고 명령을 전송하는 Center로 구성된다.


## Center

### 1. 기능 
- Agent 관리
  - 현재 접속 중인 Agent 를 관리한다. 
- 파일 전송 
  - FTP Server 형태로 파일을 전송한다.
- 원격 파일 실행 
  - 전달 한 파일을 실행 시킨다.
- 파일 실행 결과 출력
  - 엑셀 및 텍스트 파일 포맷 지원 
- 로그 조회 및 기록  
  - 파일 전송 및 실행 로그

### 2. 구조
- GUI(QT) 응용프로그램 
- MSI 설치파일 지원 

</br>

## Agent 

### 1. 기능
- 파일 전송
  - FTP Client 형태로 파일을 전송 받는다.
- 원격 파일 실행
  - Center로 부터 명령을 전달 받아 파일을 실행 시킨다.
- 유효성 검사
  - 파일 실행 전 hash 값과 실행 후 hash 값  복구 TOOL 실행 후 hash 값을 비교한다.
- 리포트 기능 
  - 유효성 검사 기능 결과를 서버에 보고한다. 
### 2. 구조 
- 윈도우 서비스 형태 개발
- MSI 설치 형태 지원

</br>

## 비고 
- QT 공부와 Network Socket 프로그래밍 공부를 위해 시작한 프로젝트 입니다. 


## 개발 기간 : 2023-02-15 ~ 2023-07-01
1. 1주차 (2-20 ~ 2-26)  
   - QT 기본 공부
     - 다이얼로그 및 위젯 사용 


