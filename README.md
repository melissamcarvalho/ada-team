# ada-team

- [ada-team](#ada-team)
- [Environment](#environment)
  - [Start the container](#start-the-container)
  - [Run the notebook inside the container](#run-the-notebook-inside-the-container)
- [Next steps](#next-steps)
- [Contributing Guide](#contributing-guide)

The goal of the hackathon was to predict the probability of a customer visit
a market store on the next 7 days based on historical data from four months.

This initial structure of this repo was inspired by the structure provided by
Kedro. 

The main resources are the following:

[Raw dataset](https://www.kaggle.com/c/marketcohackaton/data).

Please, download it and place at `ada-marketco/data`

[Jupyter notebook](reproduction of the experiments)

In order to reproduce it, you may run it inside a container Docker.
For that, first, create the Docker image

# Environment

```
cd docker
build_docker.sh
```

## Start the container

In order to map the complete project to the container, please, make sure to
apply a cd command, to move one level up.

```
docker run -it --rm -v $PWD/:/workspaces --name=ada_env -p 8888:8888 ada_env /bin/bash 
```

## Run the notebook inside the container

```
jupyter notebook --ip 0.0.0.0 --no-browser --allow-root
```

On the jupyter notebook navigate to `ada-marketco/notebooks` for running
the reproduction steps.

# Next steps

As next steps we are going to improve the feature engineering and modeling process,
and the documentation as well. Keep in touch!!

# Contributing Guide

Feel free to make a Pull Request to our development branch for suggestions on how
to make this work evn more fun! Enjoy!!