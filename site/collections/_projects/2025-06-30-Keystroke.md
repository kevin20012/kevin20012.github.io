---
date: 2025-06-30 08:20:35 +0300
title: 사용자별 키스트로크 다이나믹스를 활용한 사용자 분류 모델 개발
subtitle: 팀프로젝트
image: '/images/keystroke/predict.gif'
---

![Result](/images/keystroke/predict.gif){: width="1200" height="900"}

사용자마다 키보드 타이핑 리듬이 다른 것에서 착안하여 이를 이용해 새로운 보안 솔루션을 개발했습니다. 키보드 타이핑 데이터를 얻기 위해 tkinter로 프로그램 개발 후 4명의 팀원으로부터  '키 사이의 시간 간격', '키를 눌렀다떼는 시간', '키코드' 3가지 특징을 얻어냈습니다. 이후 탐색적 데이터 분석(EDA)를 통해 데이터를 전처리하고, 트랜스포머 및 LSTM 모델 및 앙상블 기법을 적용하여, 최종적으로 유저 분류정확도 99%를 달성하였습니다.

[GitHub Repository](https://github.com/kevin20012/KeystrokeDynamics-With-Transformer)