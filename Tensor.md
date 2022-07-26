[참고] https://tutorials.pytorch.kr/beginner/basics/tensorqs_tutorial.html  

## PyTorch  
PyTorch는 Python을 위한 오픈소스 머신 러닝 라이브러리이다.  
Torch를 기반으로 하며, 자연어 처리와 같은 애플리케이션을 위해 사용된다.  
GPU 사용이 가능하기 때문에 속도가 상당히 빠르다.  

## Tensor  
Tensor는 배열이나 행렬과 매우 유사하고 특수한 자료구조이다.  
PyTorch에서는 텐서를 사용하여 모델의 입력과 출력, 그리고 모델의 매개변수들을 부호화한다.  
텐서는 GPU나 다른 하드웨어 가속기에서 실행할 수 있다는 점만 제외하면 Numpy의 ndarray와 유사하다.  
실제로 텐서와 numpy 배열은 종종 동일한 내부 메모리를 공유할 수 있어 데이터를 복수할 필요가 없다.  
텐서는 또한 자동 미분에 최적화되어 있다.  

## Tensor 생성 
[참고] https://bigdatadiary0819.tistory.com/60 
- torch.rand(): 0과 1사이의 숫자를 균등하게 생성  
- torch.rand_like(): 사이즈를 튜플로 입력하지 않고 기존의 텐서로 정의  

## PyTorch vs tensorflow
- PyTorch: 서비스용으로 사용하면...? 덜 안정적 
- tensorflow: 완결성 필요, 안정적인 서빙

### 질문
(텐서 연산) 1. CPU가 아닌 GPU에서 실행하는 이유가 빠른 연산을 하기 위함?
(Numpy식의 표준 인덱싱과 슬라이싱) 2. tennsor[:, 1] // row = 전부, column =  1을 표현하는게 맞는지?  

