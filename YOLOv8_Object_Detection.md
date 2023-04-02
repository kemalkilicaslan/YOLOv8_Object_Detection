# YOLOv8 Object Detection

## Installation


```pip install ultralytics```

### Image Detection

#### CLI (Command Line Interface)

```yolo detect predict model=yolov8x.pt source="img.jpg" save=True```

#### Python

```
from ultralytics import YOLO

model = YOLO('yolov8x.pt')
results = model('img.jpg', save=True)
```

### Video Detection

#### CLI (Comman Line Interface)

```yolo detect predict model=yolov8m.pt source="vid.mp4" save=True```

#### Python

```
from ultralytics import YOLO

model = YOLO('yolov8m.pt')
results = model('vid.mp4', save=True)
```

### Live Detection

#### CLI (Command Line Interface)

```yolo detect predict model=yolov8n.pt source=0 show=True```

#### Python

```
from ultralytics import YOLO

model = YOLO('yolov8n.pt')
model.predict(source="0", show=True)
```

