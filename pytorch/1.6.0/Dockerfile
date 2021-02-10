FROM pytorch/pytorch:1.6.0-cuda10.1-cudnn7-runtime

RUN set -x && \
    apt-get update && \
    apt-get install -y libglib2.0-0 libsm6 libxext6 libxrender1 libfontconfig1 && \
    apt-get install -y vim-common && \
    apt-get install -y zip git && \
    pip install --upgrade pip && \
    pip install pillow && \
    pip install opencv-python && \
    pip install opencv-contrib-python && \
    pip install absl-py && \
    pip install tqdm && \
    pip install scipy && \
    pip install sklearn && \
    pip install xlrd && \
    pip install pandas && \
    pip install matplotlib && \
    pip install -U tensorboard && \
    pip install -U git+https://github.com/albu/albumentations && \
    pip install -U efficientnet_pytorch && \
    git clone https://github.com/Cadene/pretrained-models.pytorch.git && \
    cd pretrained-models.pytorch && \
    python setup.py install && \
    cd ../ && \
    pip install imagecodecs && \
    pip install -U git+https://github.com/Luolc/AdaBound && \
    pip install -U git+https://github.com/LiyuanLucasLiu/RAdam && \
    pip install -U git+https://github.com/zhanghang1989/ResNeSt && \
    pip install iterative-stratification
