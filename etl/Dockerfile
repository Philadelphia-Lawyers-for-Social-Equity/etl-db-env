FROM jupyter/pyspark-notebook

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

EXPOSE 8888

CMD ["sh","-c", "jupyter notebook"]