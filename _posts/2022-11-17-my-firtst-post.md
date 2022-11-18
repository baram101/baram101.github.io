---
title:  "[Dimension Reduction] Overview"
excerpt: "sample, 차원 축소 등의 기법으로 데이터 크기를 축소"

categories:
  - Machine Learning
tags:
  - [Machine Learning, ML, Dimension Reduction]

toc: true
toc_sticky: true
 
date: 2022-11-17
last_modified_at: 2022-11-17
---

### Dimension Reduction
###### Data Preprocessing
<font size="2">

**Data Integration** : 여러 source의 data를 하나의 data로 통합
**Data Cleaning** :  데이터에 존재하는 여러 문제점을 교정
**Data Transformation** : 정규화, 이산화 등의 방법으로 데이터를 변환
**Data Reduction** : 샘플링, 차원 축소 등의 기법으로 데이터 크기 축소

**Manifold Hypothesis** : 고차원 공간에 존재하는 데이터들은 실제로 그 고차원 공간 내부에 존재하는 manifold위에 존재한다는 가설
**Intrinsic Dimension** : 데이터를 잘 표현하기 위해 최소 몇 차원의 representation이 필요한가?
</font>

###### Curse of Dimensionality
<font size="2">

데이터의 차원이 높아지면 생기는 문제들. 
* 데이터에 noise 가 있을 가능성이 높음 -> 모델의 inference 성능에 악영향
* 모델의 training/inference 에 computational burden
* 모델의 generalization ability 를 달성하기 위해 더 많은 instance 가 필요함

차원의 저주를 해결하기 위해 다음과 같은 작업들이 이루어짐. 
* Domain Knowledge -> 필요한 면수만 선정
* Regularization term -> Generalization ability
* <span style="color:red">Dimension reduction</span>

**Background**
이론적으로는 variable 이 많을수록 모델의 performance 는 향상됨
그러나 , 변수 간의 dependency나 데이터에 존재하는 noise 등의 이유로 실제로는 그렇지 못함. 
목적 : 
모델에 가장 잘 맞는 variable subset 을 선정
효과 : 
Variable 간 correlation 제거
필요한 정보는 계속 가지고 있으면서 불필요한 정보를 제거
고차원 데이터의 시각화
