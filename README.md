# EDABK_YOLOV4_WeaponDetection 

## I. Tham khảo

[Github](https://github.com/ari-dasci/OD-WeaponDetection/tree/master/Weapons%20and%20similar%20handled%20objects)

[Blog](https://miai.vn/2020/05/25/yolo-series-train-yolo-v4-train-tren-colab-chi-tiet-va-day-du-a-z/)

## II. Setup hyperparameters

### 1. yolov4 config

Sử dụng file custom config: [yolov4-custom.cfg](./yolov4-custom.cfg)

- [yolo.names](./yolo.names)
- [yolo.data](./yolo.data)

Các tham số lưu ý:

- subdivisions: 32
- width: 608
- height: 608
- classes:6
- max_batches = max(num_classes*2000, 6000) = 12000
- steps=9600,10800 (bằng 0.8, 0.9 max_batches)
- filters=33 ( dòng 963, 1051, 1139). Tính bằng (num_classes+5)*3

### 3. Makefile

- GPU=1
- CUDNN=1
- OPENCV=1

## III. Kết quả chạy

### 1. File weights

[yolov4-custom_last.weights](https://drive.google.com/drive/folders/1j8IuxE9mM1FJqEwpBOwejllq90ilzqis?usp=sharing)

### 2. File logs

[yolov4.log](https://drive.google.com/file/d/1jFuoDcPgVR3Xx9ywdRtT26RAIka0Lw97/view?usp=sharing)

### 3. Loss

### 4. Test với ảnh test

