COMMANDS TO FOLLOW: - (WITHOUT USING MINIKUBE)


STEP 1 - Change your Kubectl config to docker desktop.

- kubectl config get-contexts
- kubectl config use-context docker-desktop



STEP 2 - Applying ingress-nginx server to proceed.

- kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.0.0/deploy/static/provider/cloud/deploy.yaml




STEP 3 - Now, Run basic commands.


- kubectl apply -f deployment.yaml
- kubectl get deployment -n ingress-nginx
- kubectl get pods --all-namespaces -l app.kubernetes.io/name=ingress-nginx
- kubectl apply -f service.yaml
- kubectl apply -f ingress.yaml
- kubectl get ing
- kubectl get ing -n ingress-nginx

STEP 4 - Lastly, Open Powershell -> Run following commands and edit your host file.

- cd driver
- cd etc
- notepad.exe hosts



