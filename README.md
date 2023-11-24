# OpenSW_hw1

1. Docker Image 설치<br/>
   &nbsp;버전 조건
   &nbsp;Tensorflow >= 1.3<br>
   &nbsp;Keras >= 2.1<br/>
   &nbsp;python >= 3.6<br/><br/>
   &nbsp; +)  GPU를 사용하여 학습
   이에 tensorflow/tensorflow:1.8.0-devel-gpu-py3를 사용<br/>
   &nbsp;link : https://hub.docker.com/layers/tensorflow/tensorflow/1.8.0-devel-gpu-py3/images/sha256-e7d8a0a6117800cf5dad37ca8ec490750e6210f3d5136b81a53f7e4f9cb5fda4?context=explore

2. Docker Image 안에 Mask_RCNN 파일 복사<br>
&nbsp; Docker cp Mask_RCNN

3. TensorFlow가 GPU 메모리를 필요한 만큼만 할당하도록 하는 설정<br>
&nbsp; os.environ['TF_FORCE_GPU_ALLOW_GROWTH'] = 'true' 를 사용

4. requirements를 아래와 같이 수정<br>
 &nbsp; numpy
&nbsp; scipy
&nbsp; Pillow
&nbsp; cython
&nbsp; matplotlib
&nbsp; scikit-image
&nbsp; tensorflow==1.3.0
&nbsp; keras==2.0.8
&nbsp; opencv-python
&nbsp; h5py
&nbsp; imgaug
&nbsp; IPython[all]


