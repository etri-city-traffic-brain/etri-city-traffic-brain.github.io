
## 도시교통 브레인

도시교통브레인 시스템(UNIQ : Urban Network Intelligence for solving traffic Queues)은 대도시의 교통소통 최적화를 위해, 클라우드-엣지 기반 실시간 교통상황 분석 및 대규모 교통 시뮬레이션 분산처리를 통해 교통제어 지능을 제공한다.

<!--
![image](https://user-images.githubusercontent.com/3960018/215690318-a6fb1566-f662-42d3-a832-6575f814b9e2.png)
-->

<center><img src="https://user-images.githubusercontent.com/3960018/215690318-a6fb1566-f662-42d3-a832-6575f814b9e2.png" width="500" height="400"></center>


O 주요 정량적 목표
   - 교차로 통과시간 감소율 15% 이상
   - 신호 최적화 신호 교차로 개수 200개 이상
   - 멀티 에이전트 신호 최적화의 클라우드-엣지 기반 분산 처리 지원
   - 신호 최적화 시각적 분석 모듈 수 2개 이상
   - 혼잡 전파 예측 정확도 F1-score 0.85 이상
   - 교통 수요 추정 오차 MAPE　10 이하
   - 공개 SW 커미터급 개발자 50명 이상 양성
#
## 목차

[연구 내용](#연구-내용)

[연차별 연구 내용](#연차별-연구-내용)

[UNIQ 시스템 구성](#UNIQ-시스템-구성)

[UNIQ 공개 버전 다운로드](#UNIQ-공개-버전-다운로드)

[설치 및 사용 가이드](#설치-및-사용-가이드)


#
## 연구 내용
* **[도시교통 브레인 핵심 SW]** 엣지-클라우드 협업을 통한 교통 네트워크 신호최적화 기술 및 도시 전체의 파급효과를 검증하는 스케일러블 시뮬레이션 기술 개발 
* **[클라우드 엣지 기반 교통상황인지 기술]** 엣지-클라우드/엣지-엣지 간 협업을 통한 교통상황 인지 및 예측 기술 개발
* **[계층적 교통 데이터 수집․가공․통합]** 다양한 공공/민간 교통데이터를 활용하여 클라우드 기반 데이터 수집, 변환, 관리 및 시간/공간축에 따른 데이터 상호 연계 기술 개발 
* **[실시간 교통상황분석 및 시각화 도구]** 엣지-클라우드 협업기반 교통 모니터링, 교통 영향 인자별 최적 신호와의 연관 관계, 신호 최적화의 도시 전체 파급효과, 도시 간 유사 패턴의 시각적 분석을 위한 대시보드 개발
* **[클라우드-엣지 통합 인프라 및 자원 관리 도구]** 도시교통 브레인의 동적 확장이 가능한 클라우드-엣지 가상화 구조 기술, 도시교통 브레인 엣지 인프라 및 자원 관리 기술, 도시교통 브레인의 PaaS 플랫폼 기술 개발
* **[도시교통 브레인 실증]** 도시교통 브레인의 개발 결과물을 지자체 신호제어 및 교통 인프라에 적용하여 실증 
 
 
<b>이동</b> : [[연구 내용](#연구-내용)]   [[연차별 연구 내용](#연차별-연구-내용)]   [[UNIQ 시스템 구성](#UNIQ-시스템-구성)]   [[UNIQ 공개 버전 다운로드](#UNIQ-공개-버전-다운로드)]   [[설치 및 사용 가이드](#설치-및-사용-가이드)]

#
## 연차별 연구 내용 
### 1차년도
![1차년도](./1yr.png)

### 2차년도
![2차년도](./2yr.png)

### 3차년도
![3차년도](./3yr.png)

### 4차년도
![4차년도](./4yr.png)

<b>이동</b> : [[연구 내용](#연구-내용)]   [[연차별 연구 내용](#연차별-연구-내용)]   [[UNIQ 시스템 구성](#UNIQ-시스템-구성)]   [[UNIQ 공개 버전 다운로드](#UNIQ-공개-버전-다운로드)]   [[설치 및 사용 가이드](#설치-및-사용-가이드)]


#
## UNIQ 시스템 구성
<!--
![image](https://user-images.githubusercontent.com/3960018/215693424-66f000e4-c0a1-43b6-8fdb-00e86ef5dc38.png)
-->
<center><img src="https://user-images.githubusercontent.com/3960018/215693424-66f000e4-c0a1-43b6-8fdb-00e86ef5dc38.png" width="500" height="400"></center>

* 클라우드 엣지 통합 관리 서브시스템(UNIQ-MGT)
  * 도시교통 브레인 운영에 필요한 프라이빗 클라우드 및 엣지 환경과 서비스 개발/운영 기능을 제공
* 계층적 교통 데이터 관리 서브시스템(UNIQ-TDM)
  * 신호최적화를 위한 교통데이터를 구축, 관리 기능을 제공
* 클라우드 엣지 기반 교통상황인지 서브시스템(UNIQ-TSI)
  * 교차로에 설치된 영상 데이터 수집 장치를 이용하여 수집한 교통 영상 정보 분석에 기반하여 교통 상황을 인지하고 이에 대응하는 서비스를 제공
* 스케일러블 교통 시뮬레이션 서브시스템(UNIQ-SIM)
  * 대규모 도로 네트워크 환경에서 확장 가능한 교통 시뮬레이션 기능을 제공
* 교통 신호 최적화 서브시스템(UNIQ-OPT)
  * 교통 시뮬레이션, 강화학습 등을 활용하여 대규모 교통 네트워크에 대한 교통 신호 최적화 기능을 제공
* 실시간 교통상황 시각적 분석 도구 서브시스템(UNIQ-VIS)
  * 수집되는 교통 데이터, 교통 시뮬레이션, 신호 최적화 등에 대한 시각적 분석 기능을 제공 

<b>이동</b> : [[연구 내용](#연구-내용)]   [[연차별 연구 내용](#연차별-연구-내용)]   [[UNIQ 시스템 구성](#UNIQ-시스템-구성)]   [[UNIQ 공개 버전 다운로드](#UNIQ-공개-버전-다운로드)]   [[설치 및 사용 가이드](#설치-및-사용-가이드)]
#
## UNIQ 공개 버전 다운로드
### 3차년도 결과물 : UNIQ v1.0
* UNIQ-MGT
  * [UNIQ-MGT Dashboard](https://github.com/etri-city-traffic-brain/cloud-edge-mgmt/releases/tag/v1.0.2)
  * [UNIQ-MGT API Gateway](https://github.com/etri-city-traffic-brain/cloud-edge-mgmt-api-gateway/releases/tag/v1.0.2)
* [UNIQ-TDM](https://github.com/etri-city-traffic-brain/traffic-data-mgmt)
  * Tag 찍어 달라고 요청해야 한다.
* [UNIQ-TSI](https://github.com/etri-city-traffic-brain/edge-intelligence)
  * Tag 찍어 달라고 요청해야 한다.
* [UNIQ-SIM](https://github.com/etri-city-traffic-brain/traffic-simulator/releases/tag/traffic-simulator-v1.0)
* [UNIQ-OPT](https://github.com/etri-city-traffic-brain/traffic-signal-optimization/releases/tag/v1.5a-20221114)
* [UNIQ-VIS](https://github.com/etri-city-traffic-brain/visualization-tool/releases/tag/v2.0.1)

<b>이동</b> : [[연구 내용](#연구-내용)]   [[연차별 연구 내용](#연차별-연구-내용)]   [[UNIQ 시스템 구성](#UNIQ-시스템-구성)]   [[UNIQ 공개 버전 다운로드](#UNIQ-공개-버전-다운로드)]   [[설치 및 사용 가이드](#설치-및-사용-가이드)]
#
## 설치 및 사용 가이드
* [UNIQ-MGT](https://github.com/etri-city-traffic-brain/cloud-edge-mgmt/README.md)
* [UNIQ-TDM](https://github.com/etri-city-traffic-brain/traffic-data-mgmt/README.md)
* [UNIQ-TSI](https://github.com/etri-city-traffic-brain/edge-intelligence/README.md)
* [UNIQ-SIM](https://github.com/etri-city-traffic-brain/traffic-simulator/README.md)
* [UNIQ-OPT](https://github.com/etri-city-traffic-brain/traffic-signal-optimization/tree/master/atsc-rl/multiagent_tf2/README.md)
* [UNIQ-VIS](https://github.com/etri-city-traffic-brain/visualization-tool/README.md)

<b>이동</b> : [[연구 내용](#연구-내용)]   [[연차별 연구 내용](#연차별-연구-내용)]   [[UNIQ 시스템 구성](#UNIQ-시스템-구성)]   [[UNIQ 공개 버전 다운로드](#UNIQ-공개-버전-다운로드)]   [[설치 및 사용 가이드](#설치-및-사용-가이드)]
