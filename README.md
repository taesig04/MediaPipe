
#  MediaPipe Hand Detector

이 프로젝트는 **MediaPipe**와 **OpenCV**를 사용하여 **실시간 손 감지 및 랜드마크 추적**을 수행합니다.  
카메라 또는 동영상 파일을 입력으로 받아 손의 주요 관절 위치를 감지하고 화면에 시각적으로 표시합니다.

---

##  주요 기능

- 양손(최대 2개)까지 실시간 감지 가능
- 손가락 관절(21개 랜드마크) 시각화
- 동영상 파일 또는 웹캠 입력 지원
- 손의 움직임에 따른 추적 기능 포함

---

 🛠️ 설치 방법

1. Python 3.12가 필요합니다.
2. 필요한 라이브러리를 설치하세요:


---

## 🚀 사용 방법

### ▶️ 동영상 파일로 실행

\`\`\`bash
python hand_tracker.py
\`\`\`

\`\`\`python
# hand_tracker.py 내 설정 예시
cap = cv2.VideoCapture("hand.mp4")  # 'hand.mp4'는 손이 등장하는 동영상 파일
\`\`\`

###  웹캠으로 실행

\`\`\`python
cap = cv2.VideoCapture(0)  # 웹캠으로 전환하려면 이 줄을 사용
\`\`\`

>  ESC 키를 누르면 프로그램이 종료됩니다.

---

##  파일 구조

\`\`\`
hand_tracker.py     # 손 감지 및 시각화 메인 코드
hand.mp4            # (옵션) 손이 등장하는 샘플 영상
README.md           # 프로젝트 설명 파일
\`\`\`

---

## 🧠 사용된 기술

- [MediaPipe](https://mediapipe.dev/)
  - Hand Tracking 솔루션
- [OpenCV](https://opencv.org/)
  - 이미지 입출력 및 시각화

---

## 📸 결과 예시

> 손이 감지되면 손가락 관절 21개가 연결된 형태로 실시간 표시됩니다.

---

## 📃 라이선스

이 프로젝트는 [MIT License](https://opensource.org/licenses/MIT)를 따릅니다.

