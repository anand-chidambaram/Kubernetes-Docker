kubectl get pods  -> to get all pod information
anand.c@Anand-Chidambaram-FT4K6K2WH5 ~ % kubectl get pods
NAME                              READY   STATUS             RESTARTS   AGE
calculator-app-deployment-hd7sr   0/1     ImagePullBackOff   0          8m1s
calculator-app-deployment-nnlsr   0/1     ImagePullBackOff   0          8m1s
calculator-app-deployment-x9rnc   0/1     ImagePullBackOff   0          8m1s





kubectl get services ->  to get service information 

NAME                        TYPE        CLUSTER-IP        EXTERNAL-IP   PORT(S)        AGE
calculator-app-deployment   NodePort    192.168.194.201   <none>        80:30000/TCP   7m33s
kubernetes                  ClusterIP   192.168.194.129   <none>        443/TCP        26h


kubectl delete pods --all
anand.c@Anand-Chidambaram-FT4K6K2WH5 ~ % kubectl delete pods --all
pod "calculator-app-deployment-hd7sr" deleted
pod "calculator-app-deployment-nnlsr" deleted



 NodePort      = Permanent door created by Kubernetes
Port Forward  = Temporary tunnel created by kubectl
