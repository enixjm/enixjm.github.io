---
layout: post
title: Attention Is All You Need
subtitle: 
categories: 논문_리뷰
tags: 
sidebar:
---

## Abstract
**Transformer** 모델은 여전히 자연어 처리 분야에서 큰 인기를 끌고 있습니다. ["Attention Is All You Need"](https://arxiv.org/abs/1706.03762) 논문에서 소개된 이 모델은 전통적인 순환 신경망(RNN) 구조를 대체하며 많은 주목을 받았습니다. 이 블로그 포스트에서는 Transformer 모델의 작동 원리와 주요 구성 요소를 자세히 설명하고, 해당 논문의 주요 기여와 실제 응용 사례를 살펴보겠습니다.

## Transformer 모델의 배경

#### 전통적인 시퀀스 모델(예: RNN, LSTM)와의 비교
Transformer 모델의 도입 이전에는 Sequential한 데이터를 처리하기 위해 주로 RNN과 LSTM모델이 사용되었습니다. 이들 모델은 시퀀스의 각 요소를 순차적으로 처리하여 시계열 데이터의 맥락을 학습합니다. 하지만 이러한 접근 방식에는 몇 가지 한계가 존재합니다.
- **순차 처리의 한계**: RNN과 LSTM은 데이터를 순차적으로 처리해야 하기 때문에 **병렬 처리**가 어렵습니다. 이는 훈련 및 추론 속도를 저하시키는 요인입니다.
- **장기 의존성 문제**: 시퀀스 길이가 길어질수록, 특히 RNN의 경우 초기 시점의 정보가 뒤로 갈수록 희석되어 기억하기 어려워지는 문제가 있습니다. LSTM은 **장기 의존성 문제**를 어느 정도 완화하지만 완벽하지는 않습니다.
- **복잡한 계산 구조**: RNN과 LSTM은 복잡한 계산 구조로 인해 모델 학습이 어려울 수 있습니다.

#### Transformer 모델의 기본 아이디어
Transformer 모델의 기본 아이디어는 Self-Attention과 이를 다중으로 수행하는 **Multi-Head Attention**을 활용하여 시퀀스를 처리하는 것입니다. 이 모델은 크게 **Encoder**와 **Decoder** 두 부분으로 나누어지며, 각각의 주요 구성 요소는 다음과 같습니다.
- **Self-Attention Mechanism**: 입력 시퀀스의 각 요소가 다른 모든 요소와의 관계를 학습하여 중요도를 계산합니다.
- **Multi-Head Attention**: 여러 개의 어텐션 헤드를 사용하여 다양한 표현을 학습하고, 이를 결합하여 더 풍부한 정보를 얻습니다.
- **Positional Encoding**: 시퀀스 내에서 각 요소의 위치 정보를 포함시켜, 순서 정보를 모델에 전달합니다.

## Transformer 모델 아키텍처
"Attention is All You Need" 논문에서 소개된 Transformer 모델의 아키텍처는 Encoder-Decoder 구조로 구성되어 있습니다. 
![image](https://github.com/user-attachments/assets/e42c75f6-a387-47d3-860e-786f402dc66b)
(Transformer의 Encoder 구조만 발전시킨 것이 BERT, Decoder 구조만 발전시킨 것이 GPT임.)
#### 인코더 (Encoder)
Encoder는 N개의 동일한 레이어로 구성됩니다. 각 레이어는 Multi-Head Attention 서브레이어와 FeedForward 서브레이어로 이루어져 있습니다. <br>
<br>
**Multi-Head Attention 레이어** <br>
**피드포워드 신경망 서브 레이어** <br>
**잔차 연결(Residual Connection)과 레이어 정규화(Layer Normalization)** <br>

#### 디코더 (Decoder)
Decoder 역시 N개의 동일한 레이어로 구성됩니다. 각 레이어는 Multi-Head Attention 서브레이어, Encoder-Decoder Attention 서브 레이어, FeedForward 서브 레이어.

작성중..
