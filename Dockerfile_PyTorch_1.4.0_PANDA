FROM pytorch/pytorch:1.4-cuda10.1-cudnn7-devel
MAINTAINER SiNpcw

# Command
CMD ["echo", "PyTorch-1.4 Customized"]

RUN set -x && \
    apt-get update && \
    apt-get install -y libglib2.0-0 libsm6 libxext6 libxrender1 libfontconfig1 && \
    apt-get install -y vim-common && \
    apt-get install -y zip git && \
    apt-get install -y openslide-tools && \
    apt-get install -y python-openslide && \
    git clone https://github.com/NVIDIA/apex && \
    cd apex && \
    pip install -v --no-cache-dir ./ && \
    cd ../ && \
    pip install --upgrade pip && \
    pip install pillow && \
    pip install opencv-python && \
    pip install opencv-contrib-python && \
    pip install imagecodecs && \
    pip install tifffile && \
    pip install absl-py && \
    pip install tqdm && \
    pip install scipy && \
    pip install sklearn && \
    pip install scikit-image && \
    pip install xlrd && \
    pip install pandas && \
    pip install matplotlib && \
    pip install numba && \
    pip install -U tensorboard && \
    pip install -U git+https://github.com/albu/albumentations && \
    pip install -U efficientnet_pytorch && \
    git clone https://github.com/Cadene/pretrained-models.pytorch.git && \
    cd pretrained-models.pytorch && \
    python setup.py install && \
    cd ../ && \
    pip install catalyst[all] && \
    pip install git+https://github.com/qubvel/segmentation_models.pytorch && \
    pip install iterative-stratification && \
    pip install openslide-python && \
    pip install -U git+https://github.com/Luolc/AdaBound && \
    pip install -U git+https://github.com/LiyuanLucasLiu/RAdam && \
    pip install -U git+https://github.com/zhanghang1989/ResNeSt && \
    pip install dropblock && \
    pip install -U neptune-client && \
    pip install cleanlab

