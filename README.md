This code originaly is from: borundev / jupyter_ml_docker

I am using it as a starting point for my understanding of Anaconda and docker containers.
I will be changing it significantly so in the end it will not look like the code in Mr. Chowdhury's git repository.

I found this information in an interesting article he wrote, link below, in Dec 2020.
https://towardsdatascience.com/making-docker-and-conda-play-well-together-eda0ff995e3c
# Description

This repository contains an example of making a Docker image for a jupyter notebook server that 
has two kernels - a pytorch and a tensorflow. This comes in handy because [tensorflow 2 breaks 
tensorboard for pytorch](https://github.com/pytorch/pytorch/issues/30966) and so having both in 
the same environment is not possible.

# Usage

To run check the vairables in the file `source_environment_variables.sh` and then run 
```bash
source source_environment_variables.sh
docker-compose -f traefik/docker-compose.yml up -d
docker-compose up -d
```
