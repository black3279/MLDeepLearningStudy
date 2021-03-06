# 러닝패킷: 통계의 기초
## 11) 분산분석 ANOVA
### 분산분석(Analysis of variance, ANOVA)
- 세 개 이상의 모평균을 비교하는데에 사용되는 분석방법
- 일원분류 분산분석 : 완전 임의화된 one-way 자료 ( 관심있는 한 가지 요인 또는 처리에 몇 개의 레벨이 있어서 실험단위가 그 레벨에 임의적으로 할당되었다는 뜻) 에 사용
- 예를 들어 서울, 부산, 대구 세 도시가 있고 각 평균이 있다고 한다
- 귀무가설은 세 도시 평균이 같다 대립가설은 평균이 모두 같은 경우가 아니다
- 유의수준이란 귀무가설이 사실인데 귀무가설을 기각할 가능성이다
- 개별가설 1,2,3 ( 서울과 부산은 같다, 서울과 대구는 같다 ... )
- 전체가설에 대한 유의수준은 개별가설의 유의수준을 합해야하므로 유의수준이 커지고, ANOVA 검정을 사옹해야 한다

### 일원분류분산분석의 모형
- 일원분류분산분석의 모형은 오차항이 평균이 0 이고 표준편차가 시그마인 정규분포를 따른다고 가정한다
- 이 모형에서 모수는 각 그룹의 평균과 시그마가 된다
- 이 모형을 가정하고 우선은 F검정을 하여 처리의 평균들이 같은지 다른지 검정한 후 , 다르다는 결론이 나오면 multif=ple comparison 을 통해 어떤 레벨에서 차이를 보이는지 본다
- 편차의 분해한다
- 전체제곱합 = 처리제곱합 + 잔차제곱합
- ANOVA F검정은 요인의 레벨에 따른 변동과 같은 레벨 안에서의 변동을 비교하게 된다
- F = 샘플 표준 사이의 분산 / 같은 샘플의 개별 데이터 간의 분산
- 평균간의 차이가 전체 변동에 비해 작은 경우 F 는 작아지고 평균간의 차이가 전체변동에 비해 큰 경우 F 값이 커진다
- F 가 커지면 유의한 결과를 준다 (기각)
- 제곱합은 자료에서 나타나는 변동을 나타낸다
- 전체자유도 = 처리자유도 + 오차자유도