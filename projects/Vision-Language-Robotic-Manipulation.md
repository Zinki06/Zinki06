[Read in Korean](./Vision-Language-Robotic-Manipulation.ko.md)

# Vision-Language Robotic Manipulation

## Overview

Developed for the ICROS 2025 conference, this system lets operators control a laboratory robot arm through natural language commands paired with pointing gestures. The goal is to make multimodal manipulation intuitive for non-expert users.

## Key Capabilities

- Speech-to-text pipeline for hands-free command input
- 3D target selection from pointing gestures
- Real-time YOLO-based object detection
- MiDaS depth estimation for spatial grounding
- GPT-4o intent parsing and task planning

## Tech Stack

**Robotics**: ROS, Python  
**Computer Vision**: YOLO, MiDaS, OpenCV, MediaPipe  
**AI**: GPT-4o, Whisper  
**Hardware**: 6-DoF robot arm

## System Architecture

Audio commands are transcribed with Whisper, interpreted via GPT-4o, and fused with MediaPipe hand tracking to triangulate pointing targets. YOLO provides instance-level detection, while MiDaS supplies depth cues so ROS can plan precise trajectories for the arm.

## Highlights

- Natural language + gesture interface for intuitive control
- Multimodal fusion enables centimeter-level targeting accuracy
- Real-time processing keeps interaction responsive
- Modular design adapts to other robot platforms with minimal changes

## Outcome

- Selected for oral presentation at ICROS 2025 (Undergraduate Paper Award)
- Core research project within the Interactive Robotics Lab
- Demonstrates transferable techniques for human-robot interaction studies

## References

- [ICROS 2025 Awards Overview](https://2025.icros.org/?page_id=61)
- [DBpia Paper Entry](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE12313642)

---

[Back to main README](../README.md)
