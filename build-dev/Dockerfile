FROM python:3.6
LABEL maintainer 'Abimael <aluno at abimael.com.br'

RUN adduser www &&\
    mkdir /app && \
    mkdir /log && \
    chown www /log

USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000

ENTRYPOINT ["/usr/local/bin/python"]
CMD ["run.py"]