### Docker commands to push an image to docker hub

```
docker tag local-image:tagname new-repo:tagname
```

---


```
docker push new-repo:tagname
```

---

### Kube Control Commands

```
kubectl create <TypeOfObject, EG: deployment> <name, EG: first-app> --image=<Image ID> 
```

Create an object, in this case of deployment taking a specific image into consideration

---

```
kubectl get deployments
```

Get all deployments

---


```
kubectl get pods
```

Get all PODS

---

```
kubectl delete deployment <deployment-name>
```
Delete a deployment

---

```
kubectl expose <ObjectName, in this case deployment> <Name, first-app> --type=LoadBalancer --port=8080
```

Expose it to a port so we can access the app from outside the container

---

```
kubectl get services
```

Get all the services running for the cluster

---
 
 ```
 minikube service <Name, first-app>
 ```

It will give the address from which it can be accessible externally

---

```
kubectl scale deployment/nodeapp --replicas=3
```

Scale the deployment named `nodeapp` to 4 replicas

---

```
kubectl set image deployment/nodeapp mydockerimages=harshvaghanii/mydockerimages
```

Update the image in the container

---

```
kubectl rollout undo deployment/nodeapp
```

Undo Deployment