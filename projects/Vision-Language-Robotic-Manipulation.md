# 🦾 Vision-Language Robotic Manipulation

<div align="center">
  <a href="https://github.com/Zinki06/Vision-Language-Model-based-AI-for-Interactive-Universal-Robotic-Manipulation">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Zinki06&repo=Vision-Language-Model-based-AI-for-Interactive-Universal-Robotic-Manipulation&theme=tokyonight&hide_border=true&bg_color=0D1117" alt="Robotic Manipulation"/>
  </a>
</div>

## 📋 프로젝트 개요

**ICROS 2025 한국로봇학회 학술대회 논문 발표 선정작**

자연어 명령과 손 포인팅 제스처를 통해 로봇을 직관적으로 조작할 수 있는 Vision-Language 기반 로봇 제어 시스템입니다.

## 🎯 주요 기능

- **STT(Speech-To-Text) 기반 자연어 명령** - 음성으로 로봇에게 작업 지시
- **제스처 인식 3D 로봇 제어** - 손 포인팅으로 목표 위치 지정
- **실시간 객체 탐지 및 추적** - YOLO를 활용한 정밀한 객체 인식
- **3D 공간 깊이 추정** - MiDaS 모델로 정확한 깊이 계산
- **멀티모달 AI 통합** - GPT-4o 기반 자연어 이해 및 명령 처리

## 🛠️ 기술 스택

<p align="center">
  <img src="https://img.shields.io/badge/ROS-22314E?style=for-the-badge&logo=ros&logoColor=white"/>
  <img src="https://img.shields.io/badge/YOLO-00FFFF?style=for-the-badge&logo=yolo&logoColor=black"/>
  <img src="https://img.shields.io/badge/MiDaS-FF6B6B?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/GPT--4o-412991?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/MediaPipe-0097FF?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white"/>
</p>

## 🏗️ 시스템 아키텍처

```
음성 입력 → STT → GPT-4o (자연어 처리)
                      ↓
실시간 카메라 → YOLO (객체 탐지) → MiDaS (깊이 추정)
                      ↓
손 제스처 → MediaPipe (포인팅 인식) → 3D 좌표 계산
                      ↓
              ROS → 로봇팔 제어
```

## 💡 핵심 혁신점

1. **직관적 인터페이스**: 복잡한 프로그래밍 없이 자연어와 제스처로 로봇 조작
2. **멀티모달 융합**: 음성, 시각, 제스처 정보를 통합한 지능형 제어
3. **실시간 처리**: 지연 없는 실시간 로봇 응답 시스템
4. **확장성**: 다양한 로봇 플랫폼에 적용 가능한 모듈식 설계

## 📊 성과

- **ICROS 2025** 제40회 한국로봇학회 학술대회 논문 발표자 선정
- **Interactive Robotics Lab** 연구 프로젝트로 진행
- **Human-Robot Interaction** 분야 핵심 기술 구현

## 🔗 관련 링크

- [GitHub Repository](https://github.com/Zinki06/Vision-Language-Model-based-AI-for-Interactive-Universal-Robotic-Manipulation)
- [ICROS 2025 Conference](http://icros.org/)
- [Interactive Robotics Lab](https://sites.google.com/view/interactive-robotics-lab)

---

<div align="center">
  <a href="../README.md">🏠 메인으로 돌아가기</a>
</div> 