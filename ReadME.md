# DeepFake Detection Solution

<p align="center">
   <img width="600" alt="스크린샷 2025-04-07 오후 1 24 28" src="https://github.com/user-attachments/assets/59a8dc65-662b-4a95-a29f-409b610fcad0" />
</p>

## 📋 프로젝트 개요

인공지능 기술을 활용하여 조작된 영상(딥페이크)을 탐지하는 웹 기반 솔루션입니다. 딥러닝 모델인 Xception 아키텍처를 기반으로 구현되었으며, 사용자가 업로드한 영상의 진위 여부를 높은 정확도로 판별합니다.

[프로젝트 데모 영상](https://www.youtube.com/watch?v=WC1znYaKgjg) << check this youtube link

## ✨ 주요 기능

- **비디오 분석**: 업로드된 비디오 파일의 프레임 분석
- **딥페이크 탐지**: 프레임별 딥페이크 확률 계산
- **결과 시각화**: 분석 결과를 직관적인 차트로 표시
- **다양한 모델 지원**: 사용자가 여러 탐지 모델 중 선택 가능
- **프레임 조절**: 분석할 프레임 수 조절 기능

## 🛠️ 기술 스택

- **백엔드**: Python, FastAPI
- **프론트엔드**: HTML, CSS
- **AI 모델**: Xception CNN 아키텍처
- **주요 라이브러리**: dlib, NumPy, OpenCV

## 📊 AI 모델 아키텍처

<p align="center">
  <img width="800" alt="Model Architecture" src="https://github.com/user-attachments/assets/b49e06ce-dc62-454b-8eae-decfa952ab40" />
</p>

Xception 모델을 기반으로 한 딥페이크 탐지 아키텍처를 구현했습니다. 이 모델은 깊이별 분리 가능한 컨볼루션(depthwise separable convolution)을 활용하여 효율적인 학습과 추론이 가능합니다.

**참고 자료**:
- [Deepfake-Detection](https://github.com/HongguLiu/Deepfake-Detection)
- [FaceForensics](https://github.com/ondyari/FaceForensics)

## 🔍 학습 결과

FaceForensics++ 데이터셋과 아시아인 얼굴 데이터셋을 활용하여 모델을 학습했습니다.

<p align="center">
  <img width="535" alt="Model Training Results" src="https://github.com/user-attachments/assets/3524d143-b2a4-4727-9088-27f657125b10" />
</p>

## 📁 프로젝트 구조
<img width="454" alt="스크린샷 2025-04-07 오후 1 36 47" src="https://github.com/user-attachments/assets/d92cb85e-4d15-4123-9da6-a342b56b0378" />


## ⚙️ 설치 및 실행 방법

### 필요 조건
- Python 3.8 이상
- pip 패키지 관리자

### 설치 과정
1. 저장소 클론
- git clone https://github.com/dannydaniel82/Deepfake-Detection-Solution.git
- cd Deepfake-Detection-Solution

2. 가상환경 설정 및 패키지 설치
- python -m venv venv
- source venv/bin/activate # Windows: venv\Scripts\activate
- pip install -r requirements.txt

**macOS 사용자를 위한 추가 설치**
- pip install boost
- pip install dlib
- pip install python-multipart
- pip install numpy==1.24.4

3. 서버 실행
- uvicorn main:app

4. 브라우저에서 `http://127.0.0.1:8000` 접속

## 📱 서비스 스크린샷

<div align="center">
<img width="600" alt="초기화면" src="https://github.com/user-attachments/assets/c159b893-f14f-4272-9635-6059e476c617">
<p>메인 화면</p>
  
<img width="600" alt="비디오 업로드" src="https://github.com/user-attachments/assets/ee3df41e-8107-44a9-9a4a-a74308c087d8">
<p>비디오 업로드 화면</p>

<img width="600" alt="모델 및 프레임 설정" src="https://github.com/user-attachments/assets/ccb85fbf-0d5b-432d-8a4f-56599f0724a9">
<p>모델 및 프레임 설정 화면</p>

<img width="600" alt="최종결과" src="https://github.com/user-attachments/assets/0276fde7-57da-4a79-a93f-a5e0f6d6f88e">
<p>분석 결과 화면</p>
</div>


## 📄 라이센스
This project is distributed under the MIT license.










