# voice_chat_ui_streamlit
음성인식 챗봇, Steamlit을 활용해 web ui를 제작함

# 설치 라이브러리

```
pip install streamlit
pip install python-dotenv
pip install streamlit-audiorecorder
```

# windows용 ffmpeg을 설치합니다.

## ffmpeg 지원 기능

    - 다양한 멀티미디어 파일과 스트림을 처리할 수 있는 오픈소스 소프트웨어
    - 비디오 및 오디오 변환 시 사용, 다양한 포맷간 변환 지원
    - 비디오 편집 :  비디오 파일의 일부분을 자르거나, 여러 비디오 파일을 하나로 합치는 기능
    - 오디오, 미디오 추출 : 비디오 파일에서 오디오 추출, 프레임 단위로 이미지 추출 지원
    - 자막 추가 : 비디오 파일에 자막 추가
    - 스트리밍 : 실시간 스트리밍 설정가능

## ffmpeg 설치 방법

1. Window PowerShell을 관리자 권한으로 실행합니다.

2. 다음 명령으로 Chocolatey를 설치합니다.

```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```

3. choco 명령으로 ffmpeg를 설치합니다.

```
choco install ffmpeg
```

# conda 환경에서 pip 라이브러리 파일만들기

- requirements.txt 파일 생성

```
pip list --format=freeze > requirements.txt
```

- 파이썬 라이브러리 한번에 설치하기

```
pip install -r requirements.txt
```

- requirements 파일을 다른 OS에서 설치를 할 경우 삭제하기

```
pywin32, pywinpty - 윈도우 전용 패키지
```
