FROM PYTHON:3.6-slim
COPY ./app.py /deploy/
COPY ./requirements.txt /deploy/
COPY ./lr_reg.pkl /deploy/
COPY ./scaler.pkl /deploy/
COPY ./templates /deploy/templates
WORKDIR /deploy/
RUN pip install -r requirements.txt
EXPOSE 80
ENTRYPOINT ["python3", "app.py"]