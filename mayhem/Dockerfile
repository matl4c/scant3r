FROM fuzzers/atheris:2.0.7-python3.9

RUN apt-get update

ADD . /src
WORKDIR /src

RUN python3 -m pip install .
RUN chmod +x /src/mayhem/fuzz-scant3r.py

CMD ["/src/mayhem/fuzz-scant3r.py"]
