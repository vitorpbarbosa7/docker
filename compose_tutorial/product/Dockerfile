#https://www.youtube.com/watch?v=Qw9zlE3t8Ko

# use non-build python image because is now working in arm64
# https://stackoverflow.com/questions/68984133/error-failed-to-solve-with-frontend-dockerfile-v0-failed-to-create-llb-definit
FROM python:3.8
COPY . /
COPY . /usr/src/app

RUN python3 -m pip install -r /usr/src/app/requirements.txt

CMD ["python3", "api.py"]
#CMD ["/bin/bash", "sleep.sh"]
