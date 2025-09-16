# Vision-Language 로봇 조작 시스템

## 프로젝트 개요

ICROS 2025 한국로봇학회 학술대회 발표작입니다. 자연어 명령과 손 포인팅 제스처를 통해 로봇을 직관적으로 조작하는 Vision-Language 기반 로봇 제어 시스템을 개발했습니다.

## 주요 기능

- STT 기반 음성 명령 처리
- 손 포인팅 제스처로 3D 좌표 지정
- YOLO를 활용한 실시간 객체 탐지
- MiDaS 모델로 깊이 추정
- GPT-4o 기반 자연어 이해

## 기술 스택

**Robotics**: ROS, Python
**Computer Vision**: YOLO, MiDaS, OpenCV, MediaPipe
**AI**: GPT-4o, Whisper
**Hardware**: 6-DOF 로봇팔

## 시스템 구조

음성 입력과 손 제스처를 동시에 처리하여 로봇팔을 제어합니다. STT로 변환된 음성 명령을 GPT-4o로 분석하고, MediaPipe로 손 위치를 추적하여 3D 좌표를 계산합니다. YOLO로 객체를 탐지하고 MiDaS로 깊이를 추정하여 ROS를 통해 로봇팔에 전달합니다.

## 핵심 특징

- 자연어와 제스처를 결합한 직관적인 로봇 제어
- 멀티모달 정보 융합으로 정밀한 조작 가능
- 실시간 처리로 자연스러운 인터랙션
- 모듈식 설계로 다양한 로봇에 적용 가능

## 성과

- ICROS 2025 한국로봇학회 학술대회 논문 발표 선정
- Interactive Robotics Lab 연구 프로젝트 수행
- Human-Robot Interaction 분야 핵심 기술 구현

## 참고 자료

- [ICROS 2025 시상 안내](https://2025.icros.org/?page_id=61)
- [DBpia 논문 페이지](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE12313642)

---

[메인으로 돌아가기](../README.md) 
