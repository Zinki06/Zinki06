[Read in Korean](./Vibe-HandTune-with-LLM.ko.md)

# Vibe-HandTune with LLM

## Overview

Vibe-HandTune is an interactive EDM performance tool that blends real-time hand gestures with voice prompts. The system combines MediaPipe hand tracking and large language models to let artists sculpt sound without traditional controllers.

## Key Features

- Real-time gesture recognition powered by MediaPipe Hands
- Independent control per hand (left: bass dynamics, right: lead synth parameters)
- TouchDesigner-driven visuals that react to motion data
- Whisper speech commands for quick preset switching
- MIDI output pipeline for DAW integration

## Tech Stack

**Computer Vision**: MediaPipe, OpenCV  
**Audio & Visuals**: TouchDesigner, MIDI  
**AI**: Whisper (OpenAI)  
**Language**: Python

## Implementation Notes

### 1. Gesture Tracking
MediaPipe Hands tracks 21 landmarks per hand at 30+ FPS. Temporal smoothing keeps the signals stable for musical mapping.

### 2. Gesture-to-Music Mapping
- Left hand Y-axis → bass volume envelope
- Left hand X-axis → low-pass filter cutoff
- Right hand Y-axis → lead synth gain
- Right hand X-axis → reverb depth

### 3. Visual Feedback
TouchDesigner renders a particle field whose color and intensity follow gesture velocity, creating an immediate visual response on stage.

### 4. Voice Control
Whisper converts spoken cues to text. Keywords (e.g., "drop", "bridge") trigger parameter macros for rapid scene changes.

## Impact & Limitations

**Impact**  
- Achieved <50 ms round-trip latency for natural performance flow  
- Demonstrated a controller-free EDM workflow with high audience engagement  
- Delivered synchronized audio-visual feedback for immersive showcases

**Limitations**  
- Gesture accuracy drops under harsh lighting or occlusion  
- Complex gesture chords require user training  
- Extended sessions can cause performer fatigue

## Next Steps

- Add adaptive lighting compensation for vision robustness  
- Personalize gesture templates per performer  
- Explore VR/AR staging to extend immersion

---

[Back to main README](../README.md)
