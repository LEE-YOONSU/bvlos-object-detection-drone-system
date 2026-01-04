# 비가시권(BVLOS) 객체인식 드론 시스템

본 레포지토리는 **비가시권(BVLOS) 환경**에서 드론이 촬영한
**실시간 영상 스트리밍**을 기반으로
**YOLO 객체 인식 모델을 활용한 원격 객체 인식 및 모니터링 시스템**을 다룹니다.

본 프로젝트는 **실시간 상황 인지 및 원격 감시 목적의 연구 프로젝트**로,
객체 인식 결과를 지상국(GCS)에서 즉시 확인할 수 있는
End-to-End 드론 시스템을 구현하는 것을 목표로 합니다.

---

## 프로젝트 목적
비가시권 환경에서는 드론이 촬영한 영상을
조종자가 직접 확인하기 어렵기 때문에,
실시간 영상 전송과 객체 인식의 결합이 필수적입니다.

본 프로젝트의 주요 목적은 다음과 같습니다.
- 비가시권 환경에서의 실시간 영상 기반 상황 인지
- YOLO 기반 객체 인식 모델을 활용한 원격 객체 탐지
- 영상 전송·객체 인식·시각화를 포함한 통합 시스템 검증
- 실제 운용을 고려한 지상국 중심 모니터링 구조 설계

---

## 시스템 개요
### 전체 파이프라인
```bash
Drone Camera
     ↓
Real-Time Video Streaming (LTE / RF)
     ↓
Ground Station
     ↓
YOLO Object Detection
     ↓
Detection Visualization & Logging
```
- 드론에서 촬영된 영상은 실시간으로 지상국에 전송
- 지상국에서 YOLO 기반 객체 인식 수행
- 객체 인식 결과는 영상과 함께 시각화되어 표시

---

## HM30 NETWORK 구조도
<img width="1219" height="500" alt="HM30구조도" src="https://github.com/user-attachments/assets/27658ca0-1e8f-4d72-adbc-51304950e8fe" />

---

## 기체 세팅 사진
<img width="381" height="459" alt="스크린샷 2026-01-04 182624" src="https://github.com/user-attachments/assets/eb4606b3-fc64-454f-9936-3cda6924df38" />

---
👨‍💻 Developer
- Name: LEE YOONSU
- Contact: [GitHub](https://github.com/LEE-YOONSU)
- Project: offboard_rail_following_drone
---
## Demo Video
### 장거리 비행 영상
[![Demo Video](https://img.youtube.com/vi/KbAElI_oyT8/0.jpg)](https://youtu.be/KbAElI_oyT8)

> 🔗 [Watch on YouTube](https://youtu.be/KbAElI_oyT8)
