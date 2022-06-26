# 영상기반 차량 파손 검출 모델 프로젝트
<br>

## 1. 6/26 
### YoloV5s를 사용한 간단한 detection model
- yolov5s
- Data : 2989 ==> train : val = 8:2
- epoch : 100, batchsize : 16

<br>

## 2. 6/27
### 실제 영상에 적용을 해보니 쉐보레 로고나, sportage 등 관계 없는 부분에 bounding box를 만드는 현상 발생
