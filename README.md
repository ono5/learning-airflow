# learning-airflow

## Install
[Astro CLI](https://docs.astronomer.io/astro/cli/install-cli)

[command](https://docs.astronomer.io/astro/cli/astro-deploy)

pip install "apache-airflow[celery]==2.5.0" --constraint "https://raw.githubusercontent.com/apache/airflow/constraints-2.5.0/constraints-3.7.txt"
```
brew install astro
```

## Setup

```
astro dev init
```

## Start

```
astro dev start
```

## Stop

```
astro dev stop
```

## process

```
astro dev ps
```

## Postgres

```
cat ~/.astro/config.yaml
```

## Test

```
$ docker container ls
019a6dbf4f26   learning-airflow_39359b/airflow:latest   "tini -- /entrypoint…"   35 minutes ago   Up 35 minutes                                        learning-airflow_39359b-triggerer-1

$ docker container exec -it 019a6dbf4f26 sh
$ airflow tasks test user_processing create_table 2022-01-01
```
## Local Stack
[localstack/localstack](https://github.com/localstack/localstack)
