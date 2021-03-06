
# FastApi sample

[![CircleCI](https://circleci.com/gh/david-talabard/fastapi-sample.svg?style=svg)](https://circleci.com/gh/david-talabard/fastapi-sample)

Example of a python microservices using FastApi framework

## Requirements

- Python 3
- Virtual env
- VSCode or an other IDE
  - [Autopep8 extension](https://marketplace.visualstudio.com/items?itemName=himanoa.Python-autopep8)


## Requirements

- Python 3
- Virtual env
- VSCode or an other IDE
  - [Autopep8 extension](https://marketplace.visualstudio.com/items?itemName=himanoa.Python-autopep8)

## Features

- [x] Service documentation (Open api)
- [x] Multiple environments with dotenv
- [x] Docker
- [x] Mongo connector with Motor
- [x] Authentication check (Test with keycloak)
- [x] Authentication roles check (Test with keycloak)
- [x] CI
- [x] Unit test with pytest
- [x] Cache
- [x] Kafka producer
- [x] Kafka consumer
- [ ] Jobs with Apache Airflow

## Start

- Run `./make.sh` to build the virtual env
- Activate python virtual env :
  - For linux : `source env/bin/activate`
  - For windows : `source env/Scripts/activate`
- Copy and set `.env-sample` to `.env`, edit variables
- Run `python main.py` or use a launcher in VScode
- Access to http://127.0.0.1:8080/
- Access to http://127.0.0.1:8080/docs for swagger
- Access to http://127.0.0.1:8080/redoc for Redoc
- Set WEB_CONCURRENCY environment variable for number of workers

## Tests

- Write tests in `tests` folder
- File pattern should be `*_test.py`
- Run with the command `pytest`

## Helpfull links

- [Python virtual env](https://python-guide-pt-br.readthedocs.io/fr/latest/dev/virtualenvs.htmls)
- [Python 3](https://www.python.org/)
- [Uvicorn](https://www.uvicorn.org/settings/)
- [Starlette](https://www.starlette.io/websockets/)
- [FastAPI](https://fastapi.tiangolo.com/)
- [Apache zookeeper](https://zookeeper.apache.org/)
- [Apache Kafka](https://kafka.apache.org/)
  - [For linux](https://dzone.com/articles/how-to-configure-an-apache-kafka-cluster-on-ubuntu)
  - [For windows](https://dzone.com/articles/running-apache-kafka-on-windows-os)


## Init other micro service

- Use the script `./init_from_sample.sh`
