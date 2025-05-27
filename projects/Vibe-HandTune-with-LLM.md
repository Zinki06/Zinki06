# 🎵 Vibe-HandTune with LLM

<div align="center">
  <a href="https://github.com/Zinki06/Vibe-HandTune_withLLM">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Zinki06&repo=Vibe-HandTune_withLLM&theme=tokyonight&hide_border=true&bg_color=0D1117" alt="Vibe-HandTune"/>
  </a>
</div>

## 📋 프로젝트 개요

실시간 손 제스처를 통해 EDM 음악을 직관적으로 제어할 수 있는 인터랙티브 뮤직 시스템입니다. 양손 동작으로 리듬, 이펙트, 톤을 실시간으로 조작하여 새로운 형태의 디지털 음악 퍼포먼스를 선보입니다.

## 🎯 주요 기능

- **실시간 손 제스처 인식** - MediaPipe를 활용한 정밀한 손 포인트 추적
- **양손 독립 제어** - 왼손/오른손 각각 다른 음악 요소 조작
- **다이나믹 이펙트 제어** - 제스처에 따른 실시간 사운드 이펙트 변화
- **시각화 피드백** - TouchDesigner 기반 실시간 비주얼 피드백
- **MIDI 출력** - 외부 DAW와 연동 가능한 MIDI 신호 생성
- **LLM 통합** - Whisper 기반 음성 명령으로 추가 제어

## 🛠️ 기술 스택

<p align="center">
  <img src="https://img.shields.io/badge/MediaPipe-0097FF?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/TouchDesigner-FF3D00?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/MIDI-000000?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Whisper-00A67E?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white"/>
</p>

## 🏗️ 시스템 구조

```
웹캠 입력 → MediaPipe (손 추적)
              ↓
        제스처 분석 → TouchDesigner (시각화)
              ↓
        MIDI 신호 생성 → EDM 사운드 제어
              ↓
음성 명령 → Whisper (STT) → LLM 처리 → 추가 제어
```

## 🎮 제스처 매핑

### 왼손 제어
- **Y축 움직임**: 베이스 볼륨 조절
- **X축 움직임**: 로우 패스 필터 조절
- **손가락 개수**: 리듬 패턴 변경

### 오른손 제어  
- **Y축 움직임**: 리드 신스 볼륨 조절
- **X축 움직임**: 리버브 깊이 조절
- **손가락 개수**: 이펙트 체인 활성화

## 💡 핵심 특징

1. **무접촉 인터페이스**: 물리적 컨트롤러 없이 순수 제스처로 음악 제어
2. **실시간 처리**: 지연 없는 실시간 오디오 처리 및 피드백
3. **직관적 조작**: 자연스러운 손 움직임으로 복잡한 음악 파라미터 제어
4. **확장성**: MIDI 출력으로 다양한 DAW 및 하드웨어와 연동 가능

## 🎨 시각적 피드백

TouchDesigner를 통해 실시간으로 제공되는 비주얼 요소:
- 손 위치에 따른 파티클 시스템
- 음량에 반응하는 컬러 그라디언트
- 리듬에 동기화된 기하학적 패턴
- 이펙트 강도를 나타내는 시각적 인디케이터

## 🎵 음악적 응용

- **라이브 퍼포먼스**: DJ 세트나 라이브 공연에서 독특한 시각적 요소 제공
- **음악 교육**: 직관적인 인터페이스로 전자음악 제작 학습
- **인터랙티브 아트**: 관객 참여형 음악 설치 작품
- **접근성**: 전통적인 악기 연주가 어려운 사용자를 위한 대안

## 🔗 관련 링크

- [GitHub Repository](https://github.com/Zinki06/Vibe-HandTune_withLLM)
- [TouchDesigner 공식 사이트](https://derivative.ca/)
- [MediaPipe 문서](https://mediapipe.dev/)

---

<div align="center">
  <a href="../README.md">🏠 메인으로 돌아가기</a>
</div> 