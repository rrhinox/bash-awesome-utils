# ☸️  K8s awesome command line for day by day!

## Intro & Documentation

**What is Kubernetes?**

Kubernetes is an open source container orchestration engine for automating deployment, scaling, and management of containerized applications. The open source project is hosted by the [Cloud Native Computing Foundation (CNCF)](https://www.cncf.io/).

[Kubernetes Home](https://kubernetes.io/)

[Kubernetes Docs](https://kubernetes.io/docs/home/)

[Kubernetes GitHub](https://github.com/kubernetes/kubernetes)

## Main command
+ `kubectl get pod`
+ `kubectl get nodes`
+ `kubectl events`
+ `kubectl namespaces`
+ `kubectl api-resources`


## Example with some context

## Forcing deletion of stuck Pod (in Pending/ContainerCreating status)

`kubectl delete pod <PODNAME> --grace-period=0 --force --namespace <NAMESPACE>`

[Reference StackOverflow](https://stackoverflow.com/questions/35453792/pods-stuck-in-terminating-status)

## Create a YAML template file for a deployment or pod without creating it (ex. in CKA/CKAD exam context)

`kubectl create deployment --image=nginx nginx --dry-run=client -o yaml > nginx-deployment.yaml`

`kubectl run nginx --image=nginx --dry-run=client -o yaml`


## Execute command available on pod to check something on other app/service

`kubectl exec middleware -- nc -zv frontend-svc 80`

Example output: 

`frontend-svc (10.2.3.4:80) open`



## Working and switch contexts with custom namespace

`kubectl config use-context docker-desktop` 

Output: Switched to context "docker-desktop".

`kubectl config set-context --current --namespace default` [*]

Output: Context "docker-desktop" modified.

`kubectl.exe config get-contexts`

[*] you also add this to a custom alias in .bashrc file like this:

`alias kn="kubectl config set-context --current --namespace" `

and run the following alias with your namespace: 

`kn my-working-namespace`