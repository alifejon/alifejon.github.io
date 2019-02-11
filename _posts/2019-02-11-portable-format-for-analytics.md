---
layout: post
title:  "Portable Format for Analytics (PFA) - 데이터 분석 모델 설명"
crawlertitle: "Portable Format for Analytics (PFA) - 데이터 분석 모델 설명"
summary: "Portable Format for Analytics (PFA) 소개"
date:   2019-02-11
categories: posts
tags: 'pfa'
author: alife.dev
---

- 필요성: 데이터 분석을 위한 다양한 프레임워크와 라이브러리가 존재한다. 데이터의 크기와 특성 그리고 분석 목적에 따라 서로 다른 프레임워크나 라이브러리를 활용이 있을 수 있다. 또한 새로운 라이브러리의 출현으로 데이터 분석 코드의 구현이 달라질 수는 있다.
  - ![pfa](http://dmg.org/pfa/docs/motivation/pfatoeverything.png)
- 하지만 데이터를 분석하는 행위의 본질은 크게 변하지 않는다. 따라서 새로운 시스템이나 프레임워크, 라이브러리의 출현에 따라 변하지 않는 데이터 분석에 대한 기술이 필요하다.
  - ![ml_guide](http://dlib.net/ml_guide.svg)
- Portable Format for Analytics(PFA):  앞서 이야기한 분석 프로그램 구현과 독립적인 분석 모델에 대한 하나의 해결책으로 PFA를 활용할 수 있다. PFA는 입력/출력/액션 을 정의한 문서이다. http://dmg.org/pfa
  - 입력(input): 입력 값의 속성 이나 명칭 등을 정의
  - 출력(output): 출력 값의 속성을 정의
  - 액션(action): 출력값을 얻기 위한 입력 값에 적용할 액션(수식이나 분석 모델)을 정의
- Hadrian : 앞서 소개한 PFA에는 모델을 설명하는 문서에 대한 spec.만 존재하고 이를 실제로 구현해놓고 있지는 않다. 이를 실제로 구현한 라이브러리를 하나 소개한다.
  - https://github.com/opendatagroup/hadrian