<div align="center">

<br><br>

# Subscription Waste Detection System

<br><br><br><br>

### Student Information

| **Student No** | 22421747 |
|---------------|----------|
| **Name** | 박경진 |
| **E-mail** | 241010bgj@yu.ac.kr |

---

## [Revision History]

| Date | Version | Description | Author |
|:----|:-------:|------------:|:------|
| 2026-03-27 | 0.01 | Initial Draft | 박경진 |

<br><br><br><br>

---

# =Contents=

</div>
  
1. [Business Purpose](#1-business-purpose)  
2. [System Context Diagram](#2-system-context-diagram)  
3. [Use Case List](#3-use-case-list)  
4. [Concept of Operation](#4-concept-of-operation)  
5. [Problem Statement](#5-problem-statement)  
6. [Glossary](#6-glossary)  
7. [References](#7-references)

<br><br><br><br>

---

# 1. Business purpose
## 1.1 Project background

<div align="center">
  <img src="images/20250220_090358612_02518.png" width="45%"><br>
  <sub>[그림1]</sub>
  <img src="images/20250220_090429628_00406.png" width="45%"><br>
  <sub>[그림2]</sub>
</div>


## 1.2 Goal

본 시스템의 목표는 다음과 같다.
- 구독 서비스 사용 패턴 분석
- 사용률 기반 낭비 여부 판단
- 사용자에게 해지 또는 유지 추천 분석 제공

결과적으로, 사용자가 불필요한 소비를 줄여 효율적인 구독 관리를 할 수 있게 지원한다. 

---

# 2. System context diagram



<br><br><br><br>

---

# 3. Use Case List

### 1) 구독 서비스 등록

| 항목 | 내용 |
|------|------|
| Actor | User |
| Description | 사용자는 새로운 구독 서비스를 시스템에 등록한다. 서비스 이름, 가격, 결제일 등의 정보를 입력한다.              |

### 2) 구독 서비스 수정

| 항목 | 내용 |
|------|------|
| Actor | User |
| Description | 사용자는 기존에 등록된 구독 서비스의 정보를 수정할 수 있다.                                              |
 

### 3) 구독 서비스 삭제

| 항목 | 내용 |
|------|------|
| Actor | User |
| Description | 사용자는 더 이상 사용하지 않는 구독 서비스를 삭제할 수 있다.                                             |


### 4) 사용 여부 기록

| 항목 | 내용 |
|------|------|
| Actor | User |
| Description | 사용자는 특정 구독 서비스를 실제로 사용했는지 여부를 기록한다.                                            |


### 5) 사용률 계산

| 항목 | 내용 |
|------|------|
| Actor | System |
| Description | 시스템은 일정 기간 동안의 사용 데이터를 기반으로 사용률을 계산한다.                                        |


### 6) 낭비 여부 분석

| 항목 | 내용 |
|------|------|
| Actor | System |
| Description | 시스템은 사용률이 낮은 구독 서비스를 분석하여 낭비 여부를 판단한다.                                        |


### 7) 낭비 경고 알림

| 항목 | 내용 |
|------|------|
| Actor | System |
| Description | 사용률이 낮은 서비스에 대해 사용자에게 알림을 제공한다.                                                  |


### 8) 해지 추천

| 항목 | 내용 |
|------|------|
| Actor | System |
| Description | 사용 패턴을 기반으로 해지를 추천한다.                                                                 |


### 9) 소비 통계 제공

| 항목 | 내용 |
|------|------|
| Actor | System |
| Description | 월별 구독 비용과 사용 패턴을 분석하여 통계를 제공한다.                                                  |


### 10) 리포트 생성

| 항목 | 내용 |
|------|------|
| Actor | System |
| Description | 전체 구독 사용 패턴과 낭비 분석 결과를 요약한 리포트를 생성한다.                                         |

---

# 4. Concept of Operation

## 1) Usage Tracking
| **Purpose** | 사용 패턴 수집 |
|------------|--------------|
| **Approach** | 사용 여부 또는 시간 기록 |
| **Dynamics** | 사용자 입력 시마다 저장 |
| **Goals** | 정확한 데이터 확보 |


## 2) Waste Detection 
| **Purpose** | 낭비되는 구독 식별 |
|------------|--------------|
| **Approach** | 일정 기간 사용률 분석 |
| **Dynamics** | 주기적 분석 수행 |
| **Goals** | 불필요한 비용 절감 |


## 3) Recommendation System
| **Purpose** | 사용자 의사결정 지원 |
|------------|--------------|
| **Approach** | 사용률 기반 유지/해지 추천 |
| **Dynamics** |분석 결과 생성 시 제공 |
| **Goals** | 효율적인 구독 관리 |


# 5. Problem Statement

## Problems
- 자동 결제로 인한 불필요한 비용 발생
- 사용 여부를 고려하지 않는 기존 시스템
- 사용자 소비 패턴 분석 부족

---

## Non-Functional Requirements
- Performance: 빠른 데이터 처리 및 분석
- Usability: 직관적인 UI 제공
- Scalability: 사용자 증가 대응
- Reliability: 정확한 분석 결과 제공

---

# 6. Glossary

- Subscription: 정기 결제 서비스
- Usage Rate: 서비스 사용 비율
- Waste: 사용하지 않으면서 발생하는 비용
- Recommendation: 시스템이 제공하는 제안

---

# 7. References
(작성 필요)