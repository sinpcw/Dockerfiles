FROM pytorch/pytorch:1.5.1-cuda10.1-cudnn7-devel

RUN set -x && \
    apt-get update && \
    apt-get install -y libglib2.0-0 libsm6 libxext6 libxrender1 libfontconfig1 libgl1-mesa-dev && \
    apt-get install -y vim-common && \
    apt-get install -y zip p7zip-full git && \
    apt-get install -y openslide-tools && \
    apt-get install -y --fix-missing libvips libvips-dev && \
    git clone https://github.com/NVIDIA/apex && \
    cd apex && \
    pip install -v --no-cache-dir --global-option="--cpp_ext" --global-option="--cuda_ext" ./ && \
    cd ../ && \
    pip install --upgrade pip && \
    pip install pillow && \
    pip install opencv-python && \
    pip install opencv-contrib-python && \
    pip install imagecodecs && \
    pip install absl-py && \
    pip install tqdm && \
    pip install scipy && \
    pip install sklearn && \
    pip install scikit-image && \
    pip install xlrd && \
    pip install pandas && \
    pip install matplotlib && \
    pip install numba && \
    pip install tifffile && \
    pip install pyvips && \
    pip install openslide-python && \
    pip install -U tensorboard && \
    pip install -U git+https://github.com/albu/albumentations && \
    pip install -U efficientnet_pytorch && \
    git clone https://github.com/Cadene/pretrained-models.pytorch.git && \
    cd pretrained-models.pytorch && \
    python setup.py install && \
    cd ../ && \
    pip install git+https://github.com/qubvel/segmentation_models.pytorch && \
    pip install timm && \
    pip install -U git+https://github.com/Luolc/AdaBound && \
    pip install -U git+https://github.com/LiyuanLucasLiu/RAdam && \
    pip install -U git+https://github.com/zhanghang1989/ResNeSt && \
    pip install -U adabelief-pytorch
