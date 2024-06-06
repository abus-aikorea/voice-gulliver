# Voice-Gulliver

🌍 [한국어](README.kor.md) ∙ [English](README.eng.md) ∙ [日本語](README.jpn.md)

[![GitHub License](https://img.shields.io/github/license/abus-aikorea/voice-gulliver)](LICENSE)
[![GitHub Release](https://img.shields.io/github/v/release/abus-aikorea/voice-gulliver)](https://github.com/abus-aikorea/voice-gulliver/releases)

The best gradio web-ui for asr, translation and tts. Easy one click installation. Fully portable.


## 소개
* 보이스 걸리버는  **자막, 번역, 더빙** 통합 솔루션입니다. 
* 보이스 걸리버로 영상에 다국어 자막을 추가해 보세요. 글로벌 진출 쌉가능!
* 아침마다 월드뉴스를 시청하신다고요? 그럼, 라이브 번역기능을 이용해 보세요. 유튜브에서 보던 바로 그, 실시간 번역을 지원합니다.
* 보이스 걸리버는 UVR5에서 제공하는 **보컬 리무버** 와 Meta의 **Demucs** 엔진을 탑재하고 있습니다. 
* 보이스 걸리버는 **OpenAI Whisper** 와 **Microsoft Azure AI** 를 사용합니다.      
* 보이스 걸리버는 **원클릭**으로 손쉽게 설치할 수 있으며, Gradio Web-UI 를 제공합니다. 
* 최고 수준의 **On-Device AI보이스** 기술을 경험해 보세요.  


## 주요 기능

* `VOD` 탭
  - YouTube 다운로더, 노이즈 제거, 자막, 번역, 더빙 통합환경으로 제공
  - ffmpeg 이 지원하는 모든 비디오/오디오 포맷 사용 가능
  - 출력 오디오 포맷(wav, flac, mp3) 선택가능
  - 100개 언어에 대한 음성 인식, 자막 생성
  - PC 성능에 맞는 자막 생성 옵션 선택 가능 (Whisper Model & Compute Type)
  - 원본 영상의 BGM 과 효과음을 더빙 영상에서도 그대로 유지
  - 더빙 음성의 속도, 음량, 피치 조절 지원  
  
<p align="center">
  <img style="width: 90%; height: 90%" src="images/main_page.kor.png?raw=true" alt=""/>
</p>  


* `Live` 탭
  - 실시간 음성 인식 & 번역 지원
  - Mic, Speaker 등의 오디오 입력소스 선택 가능
  - 캡처된 오디오, 인식된 자막, 번역된 자막 저장 기능 제공

* `Batch` 탭
  - 대량의 파일을 일괄 처리



## 특징
* YouTube 동영상(mp4, webm)을 다운로드하고, 오디오 파일(mp3, wav, flac)로 저장할 수 있습니다.
* 노이즈 제거 & 보컬 분리를 통해 음성인식의 정확도를 높일 수 있습니다. **MDX-Net** 과 Meta의 **Demucs**를 이용합니다.
* **원클릭 설치**. 한 번 설치하면 추가 비용 없이 **영구적**으로 사용할 수 있습니다. ( ※ Free버전은 이용시간 **30분제한** 있음)
* **Web-UI**를 제공합니다. Google Chrome 브라우저를 권장합니다.


## 실행 환경
* OS : Windows 10/11 (64bits) **※ Linux, Mac OS는 지원하지 않습니다.**
* CPU: Intel 프로세서 2GHz 이상(또는 동급 호환)
* RAM: 4GB 이상
* HDD: 설치 중 최소 20GB의 여유 공간
* GPU: CUDA 12.1을 지원하는 **NVIDIA** 그래픽 카드 권장. VRAM 4GB 이상. 8GB 이상 권장.
* 인터넷 연결 필요(설치 및 번역 작업)


## 설치 와 실행

### step 1. 패키지 준비
* A. 유료버전
    + USB에 포함된 압축파일(**voice-gulliver-x.zip**)을 컴퓨터의 적당한 위치에 압축해제
    + 혹은, 이미 압축이 해제된 폴더(**voice-gulliver-x**)를 컴퓨터의 적당한 위치에 복사

* B. 무료버전
  + [![GitHub Release](https://img.shields.io/github/v/release/abus-aikorea/voice-gulliver)](https://github.com/abus-aikorea/voice-gulliver/releases) 로부터 최신 릴리즈 (**Source code (zip)**) 다운로드 후 압축 해제 
  + 혹은, git clone 으로 소스코드 다운로드
    
```bash
git clone https://github.com/abus-aikorea/voice-gulliver.git
```

### step 2. 프로그램 설치 및 실행
1. `configure.bat` 실행
   - Windows에 ffmpeg 과 CUDA(NVIDIA GPU를 사용하는 경우)를 설치합니다. 
   - 최초 1회만 실행하면 됩니다.
2. `start.bat` 실행
   - Voice-Gulliver 을 시작합니다. Web-UI가 자동으로 실행됩니다. 
   - 최초 실행시에는 Voice-Gulliver 설치 작업을 먼저 진행합니다. 
   - Voice-Gulliver 설치는 인터넷 연결을 필요로 하며, 시스템에 따라 설치에 1시간 이상이 소요될 수 있습니다. 
   - 설치 중에는 절대 Windows-Command 창을 종료하지 마세요.
   - 설치중 문제가 발생한 경우, installer_files 폴더를 삭제하고 start.bat를 다시 실행하세요.
#### Browser가 자동으로 실행되지 않는 경우
- Windows-Commnad 창을 종료하고, start.bat 을 다시 실행하거나
- Browser를 직접 실행하고, Windows-Command 창에 표시된 주소(예, **http://127.0.0.1:7892** )를 주소창에 입력합니다.



### 실행 화면

https://github.com/abus-aikorea/voice-gulliver/assets/161691694/bb7dd2f2-9863-49e3-bd3e-59b0b8315fca



### step 3. 프로그램 제거
* `uninstall.bat` 실행: 
  - installer_files 폴더를 제거합니다. 
  - Windows 에 설치한 ffmepg, CUDA 패키지를 제거합니다(선택할 경우)

* Voice-Gulliver은 **포터블** 설치가 기본입니다. 프로그램의 제거는 설치 폴더를 삭제하는 것으로 충분합니다.


## 주의사항
Windows Defender가 실수로 batch 파일을 트로이 목마로 인식하는 경우, 이는 종종 'False Positive'라고 불립니다. 이런 문제를 해결하기 위해서는 다음과 같은 과정을 거칠 수 있습니다.

1. 파일 예외 처리: Windows Defender에서 특정 파일이나 프로세스가 보안 검사를 건너뛰도록 설정할 수 있습니다. 이를 위해 아래의 단계를 따르세요.
   * '시작' 버튼을 클릭하고 '설정'으로 이동하세요.
   * '업데이트 및 보안'을 클릭하세요.
   * 'Windows 보안'을 선택하고 '바이러스 및 위협 보호'로 이동하세요.
   * '바이러스 및 위협 보호 설정 관리'를 클릭하세요.
   * '바이러스 및 위협 보호 설정'에서 '예외 추가'를 선택하세요.
   * '파일 또는 폴더'를 선택하고, 문제의 batch 파일을 찾아 예외로 추가하세요.
2. Windows Defender를 잠시 비활성화: 이 방법은 임시적인 해결책이 될 수 있습니다. 하지만 이 방법을 사용할 경우, 컴퓨터가 다른 위협에 노출될 수 있으므로 주의가 필요합니다.
3. 백신 소프트웨어에 문제 제보: 만약 파일이 트로이 목마가 아니라는 확신이 있다면, Microsoft에 False Positive로 제보할 수 있습니다. Microsoft는 이를 검토한 후 필요한 조치를 취할 것입니다.


## 제품 문의
* 이메일 문의: <abus.aikorea@gmail.com>
* 홈페이지: <https://abuskorea.imweb.me>
* 네이버 스마트스토어 (S/W): <https://smartstore.naver.com/abus/products/10385660040>
* 네이버 스마트스토어 (솔루션): <https://smartstore.naver.com/abus/products/10298346364>
* 아마존(미국): <https://www.amazon.com/dp/B0D5H8Z4FL>
* 아마존(일본): <https://www.amazon.co.jp/dp/B0CTHT2JH3>




## YouTube
* 제품 설명: <https://youtu.be/heEN4UIQLjc>
* 자동 자막∙번역: <https://youtu.be/uQ14hoEiI4c?si=Io9K_vIDYyeu9Z8_>
* 홈 가라오케: <https://youtube.com/playlist?list=PLwx5dnMDVC9Z8kB01tQKfzTysaCCxC3C8&si=v_GLA6Edwj_AWgHg>


## Credits
* FacebookResearch Demucs: <https://github.com/facebookresearch/demucs>
* yt-dlp: <https://github.com/yt-dlp/yt-dlp>
* gradio: <https://github.com/gradio-app/gradio>


## 저작권 정보
  <img src="images/ABUS_logo.jpg" width="100" height="100"> by [ABUS](https://abuskorea.imweb.me)

