FROM python:3.7-slim

RUN mkdir src
WORKDIR /src

COPY requirements.txt /src
RUN pip3 install notebook
RUN pip3 install --trusted-host pypi.python.org -r requirements.txt
CMD [ "jupyter", "notebook", "--port=8888", "--no-browser" , "--ip=0.0.0.0", "--allow-root"]