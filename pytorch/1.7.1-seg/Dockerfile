FROM pytorch/pytorch:1.7.1-cuda11.0-cudnn8-devel

RUN set -x && \
    apt-get update && \
    apt-get install -y libglib2.0-0 libsm6 libxext6 libxrender1 libfontconfig1 libgl1-mesa-dev && \
    apt-get install -y git build-essential gcc vim-common && \
    apt-get install -y zip p7zip-full git && \
    apt-get install -y openslide-tools && \
    add-apt-repository ppa:ubuntugis/ppa && \
    apt-get update && \
    apt-get install python-numpy gdal-bin libgdal-dev && \
    pip install --upgrade pip && \
    pip install pillow && \
    pip install opencv-python && \
    pip install opencv-contrib-python && \
    pip install imagecodecs && \
    pip install absl-py && \
    pip install tqdm && \
    pip install scipy && \
    pip install scikit-learn && \
    pip install scikit-image && \
    pip install xlrd && \
    pip install pandas && \
    pip install matplotlib && \
    pip install numba && \
    pip install tifffile && \
    pip install openslide-python && \
    pip install rasterio && \
    pip install -U tensorboard && \
    pip install -U git+https://github.com/albu/albumentations && \
    pip install -U efficientnet_pytorch && \
    git clone https://github.com/Cadene/pretrained-models.pytorch.git && \
    cd pretrained-models.pytorch && \
    python setup.py install && \
    cd ../ && \
    pip install git+https://github.com/qubvel/segmentation_models.pytorch && \
    pip install timm==0.3.2
