# Instance_Segmentation
이미지내 객체들을 Mask R-CNN을 통해 탐지합니다.
---
## 프로젝트 설명
1. RGBD 카메라 데이터를 통해 객체들의 위치를 탐지하기 전 각 객체들의 마스크 데이터를 얻기 위해 Mask R-CNN 모델을 사용하였습니다.
2. 객체 탐지에는 Classification, Semantic Segmentation, Instance Segmentaion과 같은 종류가 있는데 각각의 객체들에 대한 마스크 정보가 필요하여 Mask R-CNN모델을 사용하였습니다.
3. 본 프로젝트에서는 Torchvision 패키지를 이용하여 사전 훈련된 Mask R-CNN모델을 사용하였습니다. 따라서, Mask R-CNN을 직접 구현하지는 않았습니다.
---
## 선행조건
- Pytorch
- Torchvision
---
## 실행
- Segmentation을 진행하려는 이미지 파일을 input 폴더에 넣어주세요.
- 실행 시 src폴더에서 진행, 이때 다음과 같은 형식으로 명령어를 작성해주세요.
-  python mask_rcnn_image.py  --input ../input/data/color/20.jpg  --input뒤에 사용하려는 이미지의 경로를 입력해주세요. 임계값은 --threshold {num}으로 직접 조정하실 수 있습니다.

---
## 개발인원
1. 방건호
2. 정주호
3. 선민혁
---
## 참고자료
- https://debuggercafe.com/instance-segmentation-with-pytorch-and-mask-r-cnn/#comment-2436
