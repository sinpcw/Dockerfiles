FROM pytorch/pytorch:1.2-cuda10.0-cudnn7-runtime
MAINTAINER SiNpcw

# Command
CMD ["echo", "PyTorch-1.1.0 Customized"]

RUN set -x && \
    apt-get update && \
    apt-get install -y libglib2.0-0 libsm6 libxext6 libxrender1 libfontconfig1 && \
    apt-get install -y vim-common && \
    apt-get install -y zip git && \
    git clone https://github.com/NVIDIA/apex && \
    cd apex && \
    pip install -v --no-cache-dir ./ && \
    cd ../ && \
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
    pip install matplotlib
