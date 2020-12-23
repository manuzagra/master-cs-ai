FROM ubuntu:latest

RUN apt-get update -y && apt-get install -y tzdata pandoc texlive-xetex
RUN apt-get install -y python3-pip python-dev python3-matplotlib python3-pandas 

RUN pip3 install jupyter tabulate nbconvert

ENTRYPOINT ["jupyter", "notebook", "--notebook-dir=/opt/jupyter/notebooks/", "--ip='0.0.0.0'", "--port=8888", "--allow-root"]
