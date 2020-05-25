FROM tensorflow/tensorflow:nightly-gpu-jupyter
MAINTAINER cjgo

RUN pip install sklearn
RUN apt-get update
RUN pip install opencv-python
RUN pip install matplotlib
RUN pip install pandas
RUN pip install seaborn
RUN pip install plotly==4.7.1
RUN apt-get install -y libsm6 libxext6 libxrender-dev
RUN pip install opencv-python
RUN pip install pillow
