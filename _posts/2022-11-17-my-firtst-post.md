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

# 1. Data Reduction or Dimension Reduction
#### 1.1. Data Preprocessing
* <b>Data Integration</b> :  여러 source의 data를 하나의 data로 통합
* <b>Data Cleaning</b> :  데이터에 존재하는 여러 문제점을 교정
* <b>Data Transformation</b> : 정규화, 이산화 등의 방법으로 데이터를 변환
* <b>Data Reduction</b> : 샘플링, 차원 축소 등의 기법으로 데이터 크기 축소

#### 1.2. 
* Manifold Hypothesis : 고차원 공간에 존재하는 데이터들은 실제로 그 고차원 공간 내부에 존재하는 manifold위에 존재한다는 가설
* 데이터를 잘 표현하기 위해 최소 몇 차원의 representation이 필요한가?
 고차원 데이터에서의 문제
 * 데이터에 noise 가 있을 가능성이 높음 -> 모델의 inference 성능에 악영향
* 모델의 training/inference 에 computational burden
* 모델의 generalization ability 를 달성하기 위해 더 많은 instance 가 필요
