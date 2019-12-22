FROM jupyter/pyspark-notebook

RUN echo 

ENV GRANT_SUDO yes
USER root
RUN sudo apt-get update -y
# @note `libpq-dev` required for Python packages: `sqlalchemy` and `psycopg2`
RUN sudo apt-get install -y libpq-dev

USER jovyan
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

EXPOSE 8888

CMD ["sh","-c", "jupyter notebook"]