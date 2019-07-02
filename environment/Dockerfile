FROM registry.codeocean.com/codeocean/miniconda3:4.5.11-python3.7-cuda9.2-cudnn7-ubuntu18.04

ARG DEBIAN_FRONTEND=noninteractive

RUN conda install --yes \
      PyTorch==1.0.1 \
      h5py==2.9.0 \
      matplotlib==3.1.0 \
      pandas==0.24.2 \
    && conda clean --yes --all

RUN pip install --upgrade --no-cache-dir --upgrade-strategy=only-if-needed \
      scikit-learn==0.21.2
