# DL-Emnist

# 인공신경망 프로젝트 설명

# 설계 목표: MNIST extended dataset을 이용한 CNN 모델 최적화 및 분석 

# 프로젝트 목표: MNIST extended dataset을 이용하여 직접 설계한 CNN 또는 pretrained CNN모델을 이 용하여 학습시키고 accuracy와 inference time의 적절한 조합을 찾는다. 직접 준비한 data instance에 대해 inference 결과를 얻어 학습 데이터의 테스트 결과와  비교하고 차이를 분석한다. ○ 프로젝트 수행 방법

1. MNIST extended dataset을 분석하고 LeNet-5와 ResNet-50를 이용하여 학습하고 
결과를 비교한다. (baseline) Hyperparameter 변경을 통해 최적의 학습 결과를 얻는
다.

2. Accuracy와 학습시간, 추론시간을 고려하여 직접 설계한 네트워크와 Keras의 
pretrained model을 이용한 CNN 모델을 선정하고 학습하여 결과를 분석한다. 이때 
CNN 모델 선정 과정과 결과를 실험 및 분석 결과에 근거하여 제시한다.

3. 0 ~ 9, A ~ z 까지의 숫자/문자(총 62개)를 1인당 10개씩 손으로 쓰고 스캔하거나 사
진을 찍어 각 data instance를 모아 csv 파일 형식으로 변경하여 제출한다. 이미지는 
MNIST extended dataset과 동일한 형식으로 제작하고 CSV를 읽어 이미지로 출력하
였을 때 육안으로 충분히 구분할 수 있어야 한다.

 4. 팀별 추가 데이터에 대해 2의 모델을 이용하여 inference를 진행하고 accuracy를 구하
여 2의 테스트 결과와 비교하고 차이에 대한 이유를 기술하고 그 근거를 제시한다.


# 수행과정
가. MNIST extended dataset 개요 및 분석: 새로운 data instance를 추가하기 위한 
data format 분석 (Get the data/Discover and visualize the data) - 여러 종류의 
dataset 중 하나를 선택: 근거 제시. 

나. Dataset 분류: training/validation/test dataset으로 분배 (Prepare the data)

다. Baseline 학습 및 결과분석 (LeNet5/ResNet-50)

라. 학습에 사용할 모델 선택: 다수의 후보를 대상으로 학습 결과를 이용하여 최종 모델 
선택. 근거와 분석결과 제시. (Select and train a model) 노트북 파일에 이러한 과정
 이 나타나야 함. (직접 설계한 모델과 pre-trained model 포함)

마. 모델 최적화 및 분석: 
 - Model과 training hyperparameter의 최적화를 통해 최대 성능을 획득. 
 - 최적화 과정 제시 및 결과 분석. 학습시간, 예측시간(inference time), 정확도 측면에서 분석. -> EMNIST dataset에 포함된 test dataset을 기반으로 한 성능 평가: 주어
진 dataset에 대한 학습 최적화 결과 평가 
 - Epoch에 따른 learning curve 제시. - 각 조의 손글씨 데이터에 대한 prediction 결과 분석 -> 학습 dataset 선택을 포함
한 전반적인 CNN 개발 결과에 대한 평가
 (Fine tune the model)
