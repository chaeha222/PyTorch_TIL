## 변형(Transform)  
- 데이터가 항상 머신러닝 알고리즘 학습에 필요한 최정 처리가 된 형태로 제공되지 않으며, 변형을 해서 데이터를 조작하고 학습에 적합하게 만든다.  
- 모든 TorchVision 데이터셋들은 변형 로직을 갖는, 호출 가능한 객체(callable)를 받는 매개변수를 갖는다.  
> 매개변수의 종류: 특징을 변경하기 위한 transform & 정답(label)을 변경하기 위한 target_transform  
- FashionMNIST 특징은 PIL Image 형식이며, 정답은 정수(int)이다.  
- 학습을 하려면 정규화된 텐서 형태의 특징과 원-핫으로 부호화(encode)된 텐서 형태의 정답이 필요하다.  
- 이러한 변형을 하기 위해 ToTensor와 Lambda를 사용한다.  

## ToTensor()
- ToTensor는 PIL Image나 NumPy ndarray를 FloatTensor로 변환하고, 이미지의 픽셀의 크기 값을 [0., 1.] 범위로 비례하여 조정한다.  

## Lambda 변형(Transform)  
- Lambda 변형은 사용자 정의 람다 함수를 적용한다.