## why MoveNet
1. extremely fast
2. perfect for real time fitness applications
3. best for small device, or laptop w/o GPU
4. run faster than 50FPS
5. runs on RGB images
6. detects human joint location
7. uses MobileNet V2 (image feature extractor) + Feature Pyramid Network (decoder) + CenterNet (prediction heads with custom post-processing logics)
8. **input**: frame (video/image) as float32 tensor of shape 192x192x3
9. **output**: float32 tensor of shape 1x1x17x3 == last dimensions 1x1 (normalised (0,1)), 17 keypoints, prediction confidence (0,1)

## things we are using
1. MoveNet
2. Jupyter Notebook (.ipynb)
3. Tensorflow (prolly TFLite) == 2.4.1 [recommended]
4. OpenCV
5. Matplotlib
6. Numpy

## todo:
[done] installing MoveNet

[done] loading MoveNet using TFLite

[ ] rendering results from scratch

[ ]real time rendering, image rendering

## workings of the application
--> installing MoveNet, matplotlib, cv2, tensorflow, numpy

--> downloading model from website[2] == using tflite lightning model

--> making detections using webcam by reshaping image as input, setting input and output

--> real time image rendering from scratch

## check out these websites
1. https://tfhub.dev
2. https://tfhub.dev/google/lite-model/movenet/singlepose/lightning/3
3. https://storage.googleapis.com/movenet/MoveNet.SinglePose%20Model%20Card.pdf [modelcard]
4. https://github.com/nicknochnack/MoveNetLightning [github]
