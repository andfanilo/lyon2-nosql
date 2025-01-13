# Lyon 2 NoSQL Tutorial

Contains instructions to install and use `redis`, `mongo` and `OrientDB`, and uses `Jupyter notebook` to interact with the databases in Python or shell.

## Prerequisites

- Anaconda
- Docker Desktop (make sure to reinstall Docker Desktop so the `docker` command line works)

### Setup the conda environment

Remember to use the `Anaconda Powershell` prompt at the root of your project.

```
conda create -n nosql python=3.7
conda activate nosql
conda install -c anaconda mongo-tools
pip install jupyter jupyterlab redis pymongo
```

To run your jupyter notebook: `jupyter notebook` or `jupyter lab`

### Run Redis

In a separate command line prompt:

```
docker run -it --rm --name some-redis -p 6379:6379 redis
```

### Run MongoDB

In a separate command line prompt:

```
docker run -it --rm --name some-mongo -p 27017:27017 mongo:4
```

### Run OrientDB

In a separate command line prompt:

```
docker run -it --rm --name some-orientdb -p 2424:2424 -p 2480:2480 -e ORIENTDB_ROOT_PASSWORD=root orientdb:2.2
```

## Contributions

A huge thanks to Damien SIMONIN FEUGAS for a huge part of those NoSQL tutorials which were translated into Jupyter notebooks !
