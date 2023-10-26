# Using YOLOv8 as the Backend for Label Studio

## Introduction
There are several repositories that use YOLOv8 as the backend, but none of them worked, so I modified them to make them functional.

## Before Using
* Copy your pre-trained model 'best.pt' to this folder.
* Create an empty '.env' folder.
* Modify 'docker-compose.yaml' to match your environment for LABEL_STUDIO_BASEURL and LABEL_STUDIO_API_TOKEN.

## Quickstart
Build and start Machine Learning backend on `http://localhost:9090`


```bash
docker-compose up
```

Check if it works:

```bash
$ curl http://localhost:9090/health
{"status":"UP"}
```

Then connect running backend to Label Studio using Machine Learning settings. 

## Referenced Repositories
- https://github.com/35grain/label-studio-yolov8-backend
- https://github.com/seblful/label-studio-yolov8-backend