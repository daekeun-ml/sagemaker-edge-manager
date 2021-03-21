# SageMaker Edge Manager Example

SageMaker Edge Manager는 re:Invent 2020에 출시된 Amazon SageMaker의 새로운 서비스로 다음을 수행할 수 있습니다.

+ 엣지 디바이스 하드웨어용 커스텀 모델 준비
+ 엣지 디바이스에서 머신 러닝 추론을 효율적으로 실행하기 위한 런타임 포함
+ 디바이스가 각 모델의 데이터 샘플을 SageMaker로 안전하게 전송하여 재레이블링 및 재훈련 수행

이 서비스에는 두 가지 주요 구성 요소들이 있습니다.
+ SageMaker Edge Manager in the Cloud 
+ SageMaker Edge Agent on the Edge device
  
이 노트북은 AWS SageMaker Neo 서비스를 사용하여 사전 훈련된(pre-trained) 모델을 컴파일하는 단계를 안내합니다. 이 컴파일된 모델을 패키징한 다음 Edge Device의 에이전트(Agent)에 로드하여 예측을 수행하는 방법을 보여줍니다. 마지막으로 에이전트를 통해 모델의 입력 및 출력을 S3에 캡처하는 방법을 보여줍니다.

## License Summary
이 샘플 코드는 MIT-0 라이센스에 따라 제공됩니다. LICENSE 파일을 참조하십시오.