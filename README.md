# learn-wandb-launch
Learn how to use W&amp;B's Launch Product

## Why should I use Wandb Launch?

Specifically, you will create a job that trains a neural network, create a launch queue that will be used to submit jobs for execution on your local machine, and then create a launch agent that will poll on the queue and execute the jobs that it pops from the queue with Docker.

## Instructions

1. conda env create -n learn-wandb-launch --file env.yml 
2. python train.py to refer jobs under wandb
3. schedule job from wandb UI
4. create agent on any server with Docker (also supported for K8s, AWS Sagemaker, or Google Vertex) wandb launch-agent -e bonnefond-virginie -q "Starter queue"
5. visualise finished job under https://wandb.ai/bonnefond-virginie/learn-wandb-launch?workspace=user-bonnefond-virginie
