## Convert PyTorch Yolo to Myriad-X

### 1. Download PyTorch model (`.pt`)
Available pretrained models are here 
* [yolov5](https://github.com/ultralytics/yolov5#pretrained-checkpoints)
* [yolov7](https://github.com/WongKinYiu/yolov7#performance)
### 2. Convert `.pt` to Myriad-X `.blob` file 
Move to http://tools.luxonis.com/ and convert `.pt` to `.blob`
### 3. Run Yolo object detection model with on-device decoding
* Clone this [repo](https://github.com/luxonis/depthai-experiments/tree/master/gen2-yolo/device-decoding)
* install dependencies in `depthai-experimentals/gen2-yolo/device-decoding/requirements.txt`
* move extracted `.blob` and `.json` to directory `depthai-experiments/gen2-yolo/device-decoding/`
* Run `python3 main_api.py -m /path/to/blob -c /path/to/json`

