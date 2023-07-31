# YOLOv8 기본 다지기
YOLOv8은 Object Detection과 Segmentation 또한 동일한 API를 이용하여 구현 가능하다.
YOLOv8 프로젝트 개발 프로세스 : Data Preparation(시간이 가장 많이 소요됨) -> Loading Data -> Install YOLOv8 -> Train Model -> Predicition

Object Detection : model = YOLO("yolov8n.pt")
Object Detection : model.train(data = "data.yaml", epoch = 100, imgsz = 640)

Segmentation :  model = YOLO("yolov8n - seg.pt")
Segmentation : model.train(data = "data - seg.yaml", epoch = 100, imgsz = 640)
results = model.predict(source = "test.jpg")

위와 같이 사전학습 모델종류와 데이터 위치를 나타내는 yaml파일만 바꾸어 주면, 동일한 Python API로 둘다 구현이 가능하다.




# 
