# TFRecord Viewer

[![DeepSource](https://deepsource.io/gh/MITsVision/tfrecord-viewer.svg/?label=active+issues&show_trend=true)](https://deepsource.io/gh/MITsVision/tfrecord-viewer/?ref=repository-badge)

"How about checking your data before going deeper?"

Use TFRecord Viewer to browse contents of TFRecords with object detection/classification annotations.

The viewer runs a Flask server to provide a web gallery with annotation overlays.
I.e. you can run it on your server machine, but browse on your local machine.

The web gallery displayed with [Fotorama.io](https://fotorama.io/).

# Examples

`python3 tfviewer.py datasets/COCO/tfrecord/coco_train.record-00003-of-00100 --labels-to-highlight='car;truck;bus;motorcycle'`

![Detection example](http://cmp.felk.cvut.cz/~sulcmila/tfrecord-viewer/detection.png)


`python3 tfviewer.py datasets/imagenet/imagenet_fullres/tfrecord/train-00000-of-01024 --overlay classification`

![Classification example](http://cmp.felk.cvut.cz/~sulcmila/tfrecord-viewer/classification.png)
