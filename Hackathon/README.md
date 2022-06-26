# 영상기반 차량 파손 검출 모델 프로젝트
<br>

## 1. 6/26 
### YOLOv5s를 사용한 detection model
- yolov5s
- Data : 2989 (train : val = 8:2)
- epoch : 100, batch_size : 16

<br>

## 2. 6/27
### 실제 영상에 적용을 해보니 자동차 로고(쉐보레), 모델명(sportage), 주차장 등 차량 파손과 관계 없는 부분에 bounding box를 만드는 현상 발생
### 외부 이미지 사용하여 background image 포함시켜 False Positive 방지
- 96장 image
- 416 resize
- 총 250장으로 augmentation 후 train data에 포함
<br>
### YOLOv5s를 사둉한 detection model
- yolov5s
- Data : 3239 (train : val = 8:2)
- epoch : 300, batch_size :16 
