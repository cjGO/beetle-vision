FROM tensorflow/tensorflow:nightly-gpu
MAINTAINER cjgo

#RUN python -m pip install --upgrade pip
RUN pip install jupyterlab
RUN pip install sklearn

#Fixes import cv2 error
RUN apt-get update ##[edited]
RUN apt-get install 'ffmpeg'\
    'libsm6'\ 
    'libxext6'  -y

RUN pip install opencv-python
RUN pip install matplotlib
RUN pip install pandas
RUN pip install seaborn
RUN pip install plotly==4.7.1
RUN apt-get install -y libsm6 libxext6 libxrender-dev
RUN pip install opencv-python
RUN pip install -U keras-tuner
RUN pip install pillow

EXPOSE 8888
ENTRYPOINT ["jupyter", "lab", "--ip=0.0.0.0", "--allow-root", "--no-browser"]
