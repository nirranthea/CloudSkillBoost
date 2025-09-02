```bash
export REGION = 
```

```bash
gcloud compute instance-groups managed create dev-instance-group --template=dev-instance-template --size=1 --region=$REGION && gcloud compute instance-groups managed set-autoscaling dev-instance-group --region=$REGION --min-num-replicas=1 --max-num-replicas=3 --target-cpu-utilization=0.6 --mode=on
```