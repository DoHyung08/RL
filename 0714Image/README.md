# 7월 수업
## 이미지 생성모델, YOLO


### 언어모델
언어를 단어~형태소 단위로 자르고, 각 단위에 고유한 토큰을 부여한다. 입력값의 크기가 비정형적이므로 RNN을 이용하여 학습한다.


### 이미지 생성모델
text-to-image, image-to-image 등 여러 이미지 생성 모델이 있고, text-to-text 중 가장 최신의 것으로 stableDiffusion-3가 있음
학습 데이터를 인코더를 통해 압축하고, 디코더를 통해 이미지를 생성하는 과정을 거침.
모식도가 U자 모양인 하여 U-net

하지만, 학습 데이터의 검열과 부족으로 최신의 모델도 완벽하지 않음


### 인간 피드백을 통한 강화학습 (Reinforcement Learning Human Feedback, RLHF)

인간의 피드백(좋고 나쁨)을 생성한 이미지의 보상으로 받아 생성과정을 학습함
2개의 이미지를 생성하고 인간에게 비교하라고 하는 과정이 많이 사용된다.

#### Stable-Diffusion 1.5를 사용한 RLHF 데이터 생성과정. 
작은 데이터셋으로 인해 성능은 좋지 않았다.


![image](https://github.com/user-attachments/assets/3c952bad-4a1c-4565-a403-9228ba0bbcc5)
![image](https://github.com/user-attachments/assets/bc2d6005-7b88-485e-bc44-9741f09b7478)




### YOLO v8 Fine Tuning
교통사고 이미지 데이터를 이용해 YOLO v8을 학습시켰다.

