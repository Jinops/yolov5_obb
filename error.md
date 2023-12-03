Error `The DType <class 'numpy._IntegerAbstractDType'> could not be promoted by <class 'numpy.dtypes.StrDType'>. This means that no common DType exists for the given inputs. For example they cannot be stored in a single array unless the dtype is `object`. The full list of DTypes is: (<class 'numpy._IntegerAbstractDType'>, <class 'numpy.dtypes.StrDType'>)`

```
train: WARNING: ..\datasets\roboflow\train\images\P0032.png: ignoring corrupt image/label: The DType <class 'numpy._IntegerAbstractDType'> could not be promoted by <class 'numpy.dtypes.StrDType'>. This means that no common DType exists for the given inputs. For example they cannot be stored in a single array unless the dtype is `object`. The full list of DTypes is: (<class 'numpy._IntegerAbstractDType'>, <class 'numpy.dtypes.StrDType'>)
train: New cache created: ..\datasets\roboflow\train\labelTxt.cache
Traceback (most recent call last):
  File "D:\Code\conveyor-alignment-robot\model\yolov5_obb\train.py", line 633, in <module>
    main(opt)
  File "D:\Code\conveyor-alignment-robot\model\yolov5_obb\train.py", line 530, in main
    train(opt.hyp, opt, device, callbacks)
  File "D:\Code\conveyor-alignment-robot\model\yolov5_obb\train.py", line 213, in train
    train_loader, dataset = create_dataloader(train_path, imgsz, batch_size // WORLD_SIZE, gs, names, single_cls,
  File "D:\Code\conveyor-alignment-robot\model\yolov5_obb\utils\datasets.py", line 101, in create_dataloader
    dataset = LoadImagesAndLabels(path, names, imgsz, batch_size,
  File "D:\Code\conveyor-alignment-robot\model\yolov5_obb\utils\datasets.py", line 447, in __init__
    labels, shapes, self.segments = zip(*cache.values())
ValueError: not enough values to unpack (expected 3, got 0)
```

Error `module 'numpy' has no attribute 'int'`
```
Traceback (most recent call last):
  File "D:\Code\conveyor-alignment-robot\model\yolov5_obb\train.py", line 633, in <module>
    main(opt)
  File "D:\Code\conveyor-alignment-robot\model\yolov5_obb\train.py", line 530, in main
    train(opt.hyp, opt, device, callbacks)
  File "D:\Code\conveyor-alignment-robot\model\yolov5_obb\train.py", line 213, in train
    train_loader, dataset = create_dataloader(train_path, imgsz, batch_size // WORLD_SIZE, gs, names, single_cls,
  File "D:\Code\conveyor-alignment-robot\model\yolov5_obb\utils\datasets.py", line 101, in create_dataloader
    dataset = LoadImagesAndLabels(path, names, imgsz, batch_size,
  File "D:\Code\conveyor-alignment-robot\model\yolov5_obb\utils\datasets.py", line 453, in __init__
    bi = np.floor(np.arange(n) / batch_size).astype(np.int)  # batch index
  File "d:\Programs\anaconda3\envs\yolo_obb\lib\site-packages\numpy\__init__.py", line 338, in __getattr__
    raise AttributeError(__former_attrs__[attr])
AttributeError: module 'numpy' has no attribute 'int'
```
