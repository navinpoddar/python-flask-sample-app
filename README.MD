## Flaskr an example application written in Python/Flask

![Flask plus Codefresh](docker-flask-codefresh.jpg)

Original source code from https://github.com/pallets/flask/tree/master/examples/tutorial

## Docker instructions

To create a docker image execute: 

`docker build . -t flaskr`

To run the docker image execute:

`docker run -p 5000:5000 flaskr` and visit with your browser http://localhost:5000

To run unit tests inside the container execute:

`docker run -it flaskr /bin/sh`

and then in the new command promt run

`pip install pytest && pytest`

## To use this project in Codefresh

There is also a [codefresh.yml](codefresh.yml) for easy usage with the [Codefresh](codefresh.io) CI/CD platform.

More details can be found in [Codefresh documentation](https://codefresh.io/docs/docs/getting-started/create-a-basic-pipeline/)

## Build Badge
[![Codefresh build status]( https://g.codefresh.io/api/badges/pipeline/devops-demo/my-first-project%2Fbasic-build?type=cf-2&key=eyJhbGciOiJIUzI1NiJ9.NWY2MjgwYjEzZDMwMGNmOTA2NWNhYzg5.pfhKnU-JtutF2K6yoWjZCXHcv40UGP6-KSW1wJ25bBQ)]( https://g.codefresh.io/pipelines/edit/new/builds?id=5f6291778f1f599095012004&pipeline=basic-build&projects=my-first-project&projectId=5f6281e7fb942d217293938d)
