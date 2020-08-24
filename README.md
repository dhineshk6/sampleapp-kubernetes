# sampleapp-kubernetes

For creating deployment:

kubectl create -f deployment.yaml

For creating service:

kubectl create -f service.yaml

To host the app in external ip:

kubectl patch svc servicename -p '{"spec": {"type": "LoadBalancer", "externalIPs":["ip address"]}}'
