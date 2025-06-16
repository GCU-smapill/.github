## Smapill
![image](https://github.com/user-attachments/assets/1c2cfe7a-02cb-4dd9-9b11-d344e7dc31a4)


<h1 align="center">🩺 Smapill: AIoT 기반 실시간 복약 관리 시스템</h1>
<p align="center">
  <img src="https://img.shields.io/badge/platform-Raspberry%20Pi-red?logo=raspberrypi" />
  <img src="https://img.shields.io/badge/backend-Spring%20Boot-brightgreen?logo=springboot" />
  <img src="https://img.shields.io/badge/frontend-React%20Native-blue?logo=react" />
  <img src="https://img.shields.io/badge/status-MVP-lightgrey" />
</p>

---

## 📌 프로젝트 소개

**Smapill**은 초고령 사회를 대비해 고령자의 복약 누락, 오복용, 복용 시간 혼동 등 문제를 해결하는  
**AIoT 기반 실시간 복약 관리 솔루션**입니다.  
AI 스피커(라즈베리파이) + 스마트 전구 + 모바일 앱을 통해 복약 여부를 **음성/조명으로 확인**하고  
보호자가 **실시간으로 복약 상태를 모니터링**할 수 있도록 설계되었습니다.

---

## 🔍 프로젝트 구조

```bash
📦 smapill-project/
├── .github/                  # GitHub 설정 (Actions, Issue/PR 템플릿 등)
├── smapill-front/            # 프론트엔드 - React Native 앱
├── smapill-back/             # 백엔드 - Spring Boot 서버
├── smapill-ai-speaker/       # AI 스피커 제어 (Raspberry Pi + Python)
├── smapill-vision-ocr/       # OCR 분석 서버 (FastAPI + Google Vision)
├── smapill-bulb/             # 스마트 전구 제어용 Flask 서버
├── smapill-infra/            # 인프라 설정 (Docker, 배포 스크립트 등)
└── smapill-python/           # 테스트 및 통합용 Python 실험 코드 (Private)
```

---

## 🎯 주요 기능

| 기능 | 설명 |
|------|------|
| 🗣️ 음성 복약 확인 | "약 먹었어요" 라고 말하면 자동 인식 → 복약 완료 |
| 💡 스마트 전구 피드백 | 복약 완료 시 전구 색상 변경 → 시각적 피드백 |
| 📷 OCR 처방전 등록 | 처방전 촬영만으로 복약 정보 자동 등록 |
| 👨‍👩‍👧 보호자 연동 | 보호자가 피보호자의 복약 상태를 앱으로 실시간 확인 |
| 📱 모바일 앱 UI | 캘린더 기반 복약 관리, 사용자 전환, 보호자 승인 |

---

## 🛠 기술 스택

| 구분 | 사용 기술 |
|------|------------|
| Frontend | React Native (모바일 앱) |
| Backend | Spring Boot, FastAPI, MySQL, Redis |
| AIoT | Google OCR API, Gemini API, pyttsx3, speech_recognition |
| Infra | Raspberry Pi, Docker Swarm |

---

## 🧠 시스템 아키텍처
- 사용자가 “약 먹었어요”라고 말하면 AI 스피커가 이를 인식하고, 전구가 녹색으로 변하며 복약 완료가 시각적으로 표시됩니다.
- 처방전은 카메라로 촬영 시 Google OCR을 통해 자동으로 스케줄이 등록되며, 백엔드는 이를 기록하고 보호자에게 공유합니다.

  ```
사용자 음성 (STT)
      ↓
AI 스피커 (Raspberry Pi)
      ↓
Spring Boot 서버 → Flask 전구 제어 API
      ↓
전구 색상 변경 + 서버 기록 + 보호자 알림
```

- 복약 스케줄 등록 시: OCR 인식 → 스케줄 DB 반영  
- 음성 입력 시: 실시간 반응 → 음성/전구 피드백 → 보호자 앱 동기화

<img width="978" alt="image" src="https://github.com/user-attachments/assets/853080f3-25a2-4d61-a92a-97be66a243ca" />


---

## 🌟 기대 효과
- 복약 인증을 음성+전구+서버 기록으로 자동화 → 돌봄 인력 부담 감소
- 보호자가 외부에서도 복약 여부 실시간 확인 가능
- 오프라인에서도 동작 가능한 로컬 복약 알림 기능 예정


---

## 🖥 시연 영상

👉 [유튜브로 보기](https://youtu.be/EOiXL8MI7JM)

---

## 🔗 관련 링크
- GitHub: [https://github.com/GCU-smapill](https://github.com/GCU-smapill)
- Notion: [https://likeable-discovery-567.notion.site/gcu-smapill)

---

## 🤝 팀 소개

| 이름 | 역할 | GitHub |
|------|------|--------|
| 김진성 | 프론트엔드 | [@smileman62](https://github.com/smileman62) |
| 정명서 | 백엔드 | [@ohu-star](https://github.com/ohu-star) |
| 이윤서 | AI, IoT | [@lyssva345](https://github.com/lyssva345) |
| 방서현 | IoT | [@bbbbnag](https://github.com/bbbbnag) |

---

> “약 걱정 없는 세상, 모두가 건강하게 나이 드는 사회”를 위한 AIoT 복약 파트너 – **Smapill** 🩵

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
