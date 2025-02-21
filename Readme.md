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