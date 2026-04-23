
Solution-4: Look for the qosClass which has BestEffort value, which Pods get that don't have any memory or cpu limits or request.
kubectl get pods -n project-c13 -o custom-columns=Name:.metadata.name,Qo:.status.qosClass
