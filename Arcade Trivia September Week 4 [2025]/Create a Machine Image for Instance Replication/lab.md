```bash
export VM=
export IMAGE=
export ZONE=
```

```bash
gcloud compute machine-images create $IMAGE --source-instance=$VM --source-instance-zone=$ZONE
```