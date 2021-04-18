FROM nvidia/cuda:10.2-cudnn7-devel-ubuntu18.04
# Set up environment
RUN apt-get update && apt-get install --no-install-recommends --no-install-suggests -y curl && apt-get upgrade -y
RUN apt-get install software-properties-common apt-utils -y
RUN apt-get update -y
RUN add-apt-repository ppa:deadsnakes/ppa -y
RUN apt-get -y install python3.7 python3.7-dev python3.7-venv
RUN curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
RUN python3.7 get-pip.py
RUN pip install nltk==3.4 numpy==1.14.5 scipy==1.2.1 six==1.11.0 paddlepaddle-gpu==1.7.2.post107 pyrouge==0.1.3