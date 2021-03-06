
# Won Haeng Lee
## 안녕하세요 저는 이원행입니다.현재 서울에서 병역특례(2020.09.06 이후 전직가능)로 머신러닝 및 딥러닝 모델 개발자로 일하고 있으며 효율적인 최적화 방법을 연구하는 것에 흥미를 느끼며 나이브하게 비산되어있는 데이터를 가지고 유의미한 결과물을 얻는 일을 하고있다는 자부심을 가지고 있습니다.

---

# Work Experience.

## (주) 노매드커넥션
Model Developer
2019.02 - 현재


## GOWID 법인카드 Risk Management
2020.06 - 현재

### Description
현재 금융기준으로 법인카드를 발급/사용하지 못하는 신생 스타트업 기업에게 법인카드를 발급.  
은행 및 카드사와 다르게 대표이사 연대보증 및 질권설정을 받지 않는것이 특징이며 재무제표기반의 신용평가가 아니라 실시간스크래핑 기술을 이용합니다.  
잔고를 기반으로 카드발급 승인 및 한도를 관리하기때문에 기업의 현금흐름을 파악하고 리스크를 관리합니다.  

### What did i do
* Exchange Currenct Module 개발
  * 환율정보 웹 크롤링
  * DataFrame에서 외화계좌의 입금, 출금 잔고내역 해당 환율로 치환
* Fraud Detection & Management
  * 한도를 많이 부여받기 위해 큰 자금을 입금하는 등 고객의 이상징후를 탐지
  * 악의적인 기업을 방어하기 위해 선한 기업에게 피해가가면 안된다는 전제하에 ML/DL에 대한 모형이 아니라 Rule 기반의 트리거를 설정하여 탐지
  * 탐지된 Fraud는 단계별로 구분하며 Class형태로 관리
* Monitoring System
  * 회원사의 잔고 및 한도소진율 등을 모니터링하며 상환능력에 대한 Score를 지속적으로 업데이트하며 관리
  * 타사카드 사용금액 대비 고위드카드 사용금액을 비교하여 고위드카드 미사용고객 및 소액사용 고객을 사업부로 인계
  * 고위드카드를 사용한 지출분석하여 Benefit에 대한 니즈파악
  
### Tech Stack
Python, Web Crawling PyMySql, pandas


## 롯데카드 LOCA 프로젝트
2020.05 - 2020.06

### Description
불특정 다수를 대상으로하는 카드영업방식에서 영업시간이 5분을 초과하는 경우 카드가입률이 급격히 감소하기때문에, 최대한 간단한 질문을 통해 고객의 소비패턴을 분석하고 최적의 카드를 추천해주는 알고리즘 개발.  
다양한 factor를 기반으로 페르소나를 잘 구별해줄 수 있는 유의미한 feature를 탐지하여 영업시간을 줄여줄 수 있는 최적의 질문을 선정하였습니다.  
그 결과 성별 및 나이 외에 3개의 설문답안을 입력하면 해당 고객이 포함된 고객군의 페르소나를 선정하여 최적화된 대표카드 및 서브카드를 추천해줄 수 있었습니다.

### What did i do
* Preprocessing
  * input parameter를 생성(dimension 축소)
  * 각 변수별 분포차이 분석
  * Data normalizing
* Extract main parameter
  * feature importance 및 Pearson 상관계수 분석 후 최종 input parameter 선정
* Modeling
  * 전체 98,921명의 고객 10개의 집단으로 군집화 (K-Means clustering사용)
  * 각 페르소나별 주요 소비패턴 분석 (지출 상위n개 카테고리 등)
  * 혜택을 가장 많이 받을 수 있는 카드 추천
  
### Tech Stack.
Python, Scikit-learn, pandas, flask

## 사내 데이터플랫폼내 모델배포 프로세스 개발
2020.03 - 2020.05

### Description
Kubernetes 기반으로 구축된 사내 오픈소스 분석플랫폼인 Davinci 고도화작업.  
kubeflow를 활용하여 머신러닝 또는 딥러닝 워크플로우(pipeline)를 구축하고 배포까지 하나의 오케스트레이션을 구축하는것이 목표입니다.  


### What did i do
* Private Docker Registry 생성
* Machine learning Pipeline 구축
* Deploy and Predict Test

### Tech Stack.
Python, Scikit-learn, Keras, Docker, Kubernetes

## KAPA(한국감정평가사협회) OCR 프로젝트
2019.12 - 2020.03

### Description
감정평가원에 감정평가문서 OCR(Optical Character Recognition) 모델개발.  
Prop Tech의 기반이되는 감정평가서의 데이터를 인식하는 OCR 모델을 개발하고 추출된 정보를 템플릿화 하여 db에 적재가 가능하도록 만드는 프로젝트를 수행.  
또한, 감정평가서 OCR 프로젝트는 '감정평가 및 감정평가사에 관한 법률' 개정과 관련하여 감정평가서를 디지털화 하는 작업에 초석이 되는 프로젝트입니다.   
감정평가서의 디지털화가 추진되면 은행은 서류보관비용 절감 및 금융업무 효율성증대, 감정평가법인은 인쇄 및 발송비용 절감 등의 긍정적 효과를 기대할 수 있습니다.  

### What did i do
* 감평사 문건에 최적화된 전처리 개발
  * Table Detection Module 개발(감평서 문서내 표 검출)
  * 본문에 포함된 특수문자, 기호 인식 Module 개발
  * blur, threshold, erode, close 등의 조합으로 각 문서에 최적화된 전처리방법을 target으로하는 classification model 개발
* 인식결과 템플릿화 모듈 개발
  
### Tech Stack.
Python, OpenCV, Keras, pandas

## KB손해보험 오픈소스기반 분석플랫폼 개발
2019.03 - 2019.10

### Description
__개요__  
오픈소스 기반 분석 플랫폼 구축 및 분석모델 개발.  
KB손해보험의 대용량 데이터를 손쉽게 활용할 수 있는 분석플랫폼을 구성하여 머신러닝/딥러닝 등 다양한 분석 요구사항을 수용할 수 있는 "오픈소스 통합분석 플랫폼" 환경을 제공 및 분석모델을 KB손해보험의 레거시 시스템과 연동하는 프로젝트 연구활동  
__분석모델__
* 외국인등록증 OCR 모델 개발  
  * KB손해보험 외국인고객의 신분증(외국인등록증)이 입력되면 실무자가 직접 눈으로 확인후에 DB에 적재하는 등 단순업무 노동량이 많음  
  * 개인정보보호법에 의해 고유식별번호(외국인등록번호 등) 를 masking 해야할 필요성이 있으나 실무자별 maksing 작업의 범주가 통일되지 않음
  * 따라서 사진내에서 신분증을 식별하고 masking 작업과 classifiation 및 detection을 수행해주는 모델 개발하여 실무자의 노동강도를 줄여주고 데이터의 통일성을 확보함

### What did i do
* 외국인등록증 OCR 모델 개발
  * 앞/뒷면 classification model 개발
  * 신분증사진에 특화된 전처리 프로세스 개발
  * target label 검출을 위한 프로세스 개발
  
### Tech Stack.
Python, OpenCV, Keras, Docker
- - -

# Skills.

## Overall.
* 나이브한 데이터는 원석이라고 생각합니다. 그것을 가공하여 의미있는 산출물을 내는 일을 하고있음에 즐거움을 느낍니다.
* 모든것을 수용하는것이 배려라고 여기지 않습니다. 할 수 있는것과 그렇지 않은것에 대한 구분을 명확하게 제시하는것이 서로에 대한 배려라고 믿습니다.
* 부족함이 많음을 인정합니다. 하지만 필요한경우 적극적으로 방법을 탐색하고 주어진 상황내에 최고의 아웃풋을 위해 노력합니다.
* 스스로의 동기부여를 위해 Background(왜 이 일을 해야하는가?), Plan(무엇을 어떻게 할것인가?), Benefit(그로인해 무엇을 얻을 수 있는가?)을 찾길 원합니다.

## Communication.
* 크리티컬한 이슈가 발생했을때 보고하는것을 주저하지 않습니다.
* 침묵은 조직 전체를 병들게 한다고 믿기 때문입니다.
* 먼저 일에 착수하는것보다 충분히 논의하고 토론한 후에 업무를 시작하는것이 더 좋은 결과를 만든다고 믿습니다.

## Docker.
* Docker image를 빌드하고 배포할 수 있습니다.
* Private Registry를 생성하고 관리할 수 있습니다.
* Docker volume을 사용한 경험이 있습니다.
* 개인 개발환경을 Docker image로 관리하는 것을 선호합니다.

## ML/DL Frame Work.
* 데이터에 및 네트워크에따라 scikit-learn, keras, tensorflow를 적절히 사용합니다.
* Tensorboard를 통해 모델학습을 시각화할 수 있으며 그로인해 과적합 또는 과소적합을 판단할 수 있습니다.
* 네트워크는 도구일뿐 데이터 탐색 및 적절한 파라미터 선정, 하이퍼파라미터의 튜닝이 중요하다고 믿습니다.

## Others.
* Opencv, Pandas 등 전처리에 필요한 파이썬 라이브러리를 다룰 수 있습니다.
* Git과 같은 협업툴을 사용할 수 있습니다.
