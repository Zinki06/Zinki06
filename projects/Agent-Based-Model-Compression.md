# 🧠 Agent-Based Model Compression

<div align="center">
  <a href="https://github.com/Zinki06/Development-of-Agent-Based-Environments-for-Model-Compression">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Zinki06&repo=Development-of-Agent-Based-Environments-for-Model-Compression&theme=tokyonight&hide_border=true&bg_color=0D1117" alt="Model Compression"/>
  </a>
</div>

## 📋 프로젝트 개요

강화학습 기반 에이전트를 활용하여 대규모 언어 모델(LLM)의 자동 압축을 수행하는 연구 프로젝트입니다. 온디바이스 AI 환경에서의 효율적인 모델 배포를 목표로, 성능 손실을 최소화하면서 모델 크기를 획기적으로 줄이는 방법론을 개발했습니다.

## 🎯 주요 기능

- **강화학습 기반 자동 압축** - 에이전트가 최적의 압축 전략을 학습
- **다중 압축 기법 통합** - Pruning, Quantization, Distillation 동시 적용
- **성능 보존 최적화** - 압축 후에도 원본 모델 성능의 95% 이상 유지
- **확장 가능한 환경** - 다양한 모델 아키텍처에 적용 가능
- **실시간 모니터링** - 압축 과정 중 성능 지표 실시간 추적
- **Docker 컨테이너화** - 재현 가능한 실험 환경 제공

## 🛠️ 기술 스택

<p align="center">
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Transformers-FF6F00?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Weights%20&%20Biases-FFBE00?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white"/>
</p>

## 🏗️ 시스템 아키텍처

```
대상 LLM → 모델 분석 → 압축 에이전트 환경
              ↓
        강화학습 에이전트 → 압축 전략 결정
              ↓
      압축 기법 적용 → 성능 평가 → 보상 계산
              ↓
        최적화된 경량 모델 출력
```

## 🔬 압축 방법론

### 1. Structured Pruning
- **채널별 중요도 분석** - 각 레이어의 채널별 기여도 계산
- **블록 단위 제거** - 구조적 일관성을 유지한 pruning
- **적응적 임계값** - 레이어별 최적 pruning 비율 결정

### 2. Dynamic Quantization
- **혼합 정밀도** - 중요도에 따른 차등 quantization
- **캘리브레이션 최적화** - 대표 데이터셋 기반 정밀 조정
- **하드웨어 친화적** - 실제 배포 환경 고려한 quantization

### 3. Knowledge Distillation
- **다단계 증류** - 점진적 지식 전달로 성능 손실 최소화
- **어텐션 전이** - Transformer 구조의 어텐션 패턴 학습
- **태스크별 특화** - 특정 작업에 최적화된 student 모델

## 🎮 강화학습 환경

### State Space
- 현재 모델 구조 및 파라미터 정보
- 압축 진행률 및 성능 지표
- 메모리 사용량 및 추론 속도

### Action Space
- Pruning 비율 선택 (0-90%)
- Quantization 비트 수 결정 (4-16bit)
- Distillation 강도 조절

### Reward Function
```python
reward = α × (performance_retention) + 
         β × (compression_ratio) + 
         γ × (inference_speedup) - 
         δ × (quality_degradation)
```

## 📊 실험 결과

### 성능 비교 (BERT-Base 기준)
| 압축 방법 | 모델 크기 | 추론 속도 | 성능 유지율 |
|-----------|-----------|-----------|-------------|
| Baseline | 100% | 1.0x | 100% |
| Manual Compression | 25% | 3.2x | 87% |
| **Agent-Based** | **22%** | **4.1x** | **96%** |

### 다양한 모델에서의 검증
- **GPT-2**: 75% 압축, 성능 94% 유지
- **DistilBERT**: 60% 추가 압축, 성능 92% 유지  
- **RoBERTa**: 70% 압축, 성능 95% 유지

## 💡 핵심 혁신점

1. **자동화된 최적화**: 수동 튜닝 없이 최적 압축 전략 자동 발견
2. **다목적 최적화**: 크기, 속도, 성능을 동시에 고려한 균형점 탐색
3. **전이 학습**: 한 모델에서 학습한 압축 전략을 다른 모델에 적용
4. **하드웨어 인식**: 실제 배포 환경의 제약사항을 고려한 압축

## 📱 온디바이스 AI 적용

- **모바일 배포**: 스마트폰에서 실시간 자연어 처리
- **엣지 컴퓨팅**: IoT 디바이스에서 경량 AI 추론
- **배터리 효율성**: 전력 소비 최소화로 더 오래 사용 가능
- **개인정보 보호**: 클라우드 연결 없이 로컬에서 AI 처리

## 🔗 관련 링크

- [GitHub Repository](https://github.com/Zinki06/Development-of-Agent-Based-Environments-for-Model-Compression)
- [PyTorch Model Compression](https://pytorch.org/tutorials/recipes/recipes/tuning_guide.html)
- [ONNX Runtime](https://onnxruntime.ai/)

---

<div align="center">
  <a href="../README.md">🏠 메인으로 돌아가기</a>
</div> 