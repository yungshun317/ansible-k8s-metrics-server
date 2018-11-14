## Deploy
$ kubectl create -f metrics-server/deploy/1.8+/

$ kubectl get pods -n kube-system
NAME                                 READY   STATUS    RESTARTS   AGE
metrics-server-76db6db868-jvzrv      1/1     Running   0          78s

$ kubectl logs -n kube-system metrics-server-76db6db868-jvzrv

## Monitoring
$ kubectl top pods --all-namespaces
