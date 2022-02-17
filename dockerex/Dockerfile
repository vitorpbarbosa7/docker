FROM python:3.7.6
RUN mkdir WORK_REPO
RUN cd WORK_REPO
WORKDIR WORK_REPO
COPY requirements.txt requirements.txt
COPY src src

RUN python3 -m pip install -r requirements.txt

CMD ["python3","-u","src/main.py"]
