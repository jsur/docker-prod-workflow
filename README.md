## Docker / Travis CI / AWS practice

[![Build Status](https://travis-ci.org/jsur/docker-prod-workflow.svg?branch=master)](https://travis-ci.org/jsur/docker-prod-workflow)

### Workflow:
  - Code changes merged to `master`
  - Travis sees changes in `master`, builds dev Docker image, runs tests successfully
  - Travis deploys app to AWS Elastic Beanstalk
  - Elastic Beanstalk builds app image with prod `Dockerfile`

App deployed here: http://dockerprodworkflow-env.6bxywmx4fz.eu-central-1.elasticbeanstalk.com/ 