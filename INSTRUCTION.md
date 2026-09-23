# INSTRUCTION.md

## Apply

kubectl apply -f configMap.yml
kubectl apply -f secret.yml
kubectl apply -f deployment.yml

## Validate

kubectl get configmap -n todoapp
kubectl get secret -n todoapp
kubectl get deployment -n todoapp
kubectl get pods -n todoapp

kubectl exec -n todoapp <pod-name> -- printenv PYTHONUNBUFFERED
kubectl exec -n todoapp <pod-name> -- printenv SECRET_KEY

kubectl describe deployment todoapp -n todoapp