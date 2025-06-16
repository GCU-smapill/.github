## Smapill
![image](https://github.com/user-attachments/assets/1c2cfe7a-02cb-4dd9-9b11-d344e7dc31a4)


# 📘 Smapill - 실시간 복약 관리 IoT 시스템

Smapill은 고령자의 복약 누락 문제를 해결하기 위해 개발된 AIoT 기반 복약 관리 시스템입니다.  
AI 스피커와 스마트 전구, OCR 기술을 결합하여 음성과 조명을 통한 직관적인 복약 피드백을 제공하며,  
보호자와 실시간 연동이 가능한 원격 의료 솔루션을 제공합니다.

---

## 🚀 주요 기능
- AI 스피커로 복약 여부 음성 입력 → 자동 인식 및 확인
- 스마트 전구 색상으로 복약 여부 시각적 피드백
- Google OCR을 이용한 처방전 자동 인식 및 일정 등록
- 보호자 연동을 통한 실시간 복약 확인

---

## 🛠 기술 스택
- **Frontend**: React Native (모바일 앱)
- **Backend**: Spring Boot + FastAPI
- **Infra**: Raspberry Pi + Docker
- **AIoT**: Google OCR API, pyttsx3, speech_recognition, WiZ 전구

---

## 🧠 시스템 아키텍처
- 사용자가 “약 먹었어요”라고 말하면 AI 스피커가 이를 인식하고, 전구가 녹색으로 변하며 복약 완료가 시각적으로 표시됩니다.
- 처방전은 카메라로 촬영 시 Google OCR을 통해 자동으로 스케줄이 등록되며, 백엔드는 이를 기록하고 보호자에게 공유합니다.
<img width="978" alt="image" src="https://github.com/user-attachments/assets/853080f3-25a2-4d61-a92a-97be66a243ca" />


---

## 🌟 기대 효과
- 복약 인증을 음성+전구+서버 기록으로 자동화 → 돌봄 인력 부담 감소
- 보호자가 외부에서도 복약 여부 실시간 확인 가능
- 오프라인에서도 동작 가능한 로컬 복약 알림 기능 예정

---

## 🔗 관련 링크
- GitHub: [https://github.com/GCU-smapill](https://github.com/GCU-smapill)
- Notion: [https://likeable-discovery-567.notion.site/gcu-smapill)
- 시연 영상: [https://youtu.be/EOiXL8MI7JM](https://youtu.be/EOiXL8MI7JM)

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
