---
layout: post
title: "7일차 - 자바스크립트 엔진"
subtitle: "siotz"
categories: siotz
tags: til
comments: true
---

# 추후에 정리가 필요한 문서입니다!!!

# 7일차

1. 조시옷님의 자바스크립트 엔진

# 자바스크립트 엔진

## 1. 렌더링 엔진

### 1. 렌더링 ?

`HTML`과 `CSS`, `JS` 파일 등 해당 웹 페이지에 필요한 리소스들을 불러온 뒤 각종 처리 작업을 거쳐 실제 사용자가 보는 화면에 띄우는 작업

- Gecko - `Firefox`
- WebKit - `Safari`
- Blink - `Chrome`, `Opera` (15 버전부터)
- Trident - `익스플로러`
- EdgeHTML - `마이크로소프트 엣지`

> google Chrome은 원래 webkit을 사용했다.(그래서 css에서 접두사로 webkit 사용) 지금은 구글이 `Blink` 라는 차세대 엔진을 자체적으로 개발해서, 이 엔진을 사용하고 있다.

### 2. 렌더링 엔진의 렌더링 과정

#### 1. HTML을 파싱해 DOM 트리를 구성한다.

#### 2. CSSOM 트리 구성

**CSSOM (CSS Object Model)** : CSS 객체 모델

#### 3. 렌더 트리 구성

DOM 트리(HTML)와 CSSOM트리를 결합하여 렌더 트리를 생성한다.

#### 4. 레이아웃 또는 리플로우

#### 5 .페인트 또는 레스터라이징 (Paint or Rasterizing)

#### 6. 합성 또는 렌더(Composite or Render)

실제 브라우저 화면을 업데이트 한다.

## 이 때, 자바스크립트는 `렌더링 엔진`이 아닌 `자바스크립트 엔진`이 처리한다.

## 3. 자바스크립트 엔진
