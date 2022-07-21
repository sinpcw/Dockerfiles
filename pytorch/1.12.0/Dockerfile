FROM pytorch/pytorch:1.12.0-cuda11.3-cudnn8-devel

ENV TZ=Asia/Tokyo
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN set -x && \
    apt-get update && \
    apt-get install -y libglib2.0-0 libsm6 libxext6 libxrender1 libfontconfig1 libgl1-mesa-dev && \
    apt-get install -y git build-essential gcc vim-common && \
    apt-get install -y zip p7zip-full git libopencv-dev && \
    apt-get install -y python-openslide openslide-tools && \
    apt-get update && \
    apt-get install -y python-numpy gdal-bin libgdal-dev && \
    pip install --upgrade pip && \
    pip install ipywidgets && \
    pip install pillow && \
    pip install opencv-python && \
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
    pip install rasterio && \
    pip install openslide-python && \
    pip install h5py && \
    pip install pycocotools && \
    pip install -U tensorboard && \
    pip install -U git+https://github.com/albu/albumentations && \
    pip install git+https://github.com/rwightman/pytorch-image-models.git && \
    pip install librosa && \
    pip install SoundFile && \
    pip install lap && \
    pip install imagehash && \
    pip install pytorch_metric_learning && \
    pip install fastdist && \
    pip install ftfy && \
    pip install regex && \
    pip install git+https://github.com/openai/CLIP.git
