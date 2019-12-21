# k8sworkshop

Yaml files for kubernetes workshop  
The code for applications we hosted using k8s is available at https://github.com/dheeraj-blinds/docker-Task  
Deck for k8s https://prezi.com/view/NHG6MYoaYI8vxgmAnqQN/  


Following are the commands that we used during the workshop   
****** Kubectl commands **********       
 kubectl help  
 kubectl config  
 kubectl config current-context  
 kubectl get api-resources  
 kubectl api-resources  
 kubectl explain pod  
 kubectl explain pod.spec  
 kubectl explain pod.spec.containers  
 kubectl create namespace gcc  
 kubectl get namespaces  
 kubectl apply -f .\1-kubectl\example.yaml  
 
 ******** pod commands ************  
 kubectl apply -f .\2-pod\solution\1.yaml    
 kubectl get pods  
 kubect log hello-world  
 kubectl log hello-world  
 kubectl logs hello-world  
 kubectl describe hello-world  
 kubectl describe pod hello-world  
 kubectl get pods -selector=type=front-end  
 kubectl get pods --selector=type=front-end  
 kubectl get pods --selector=name=asia   
 kubectl delete -f .\1-kubectl\example.yaml    
 kubectl get pods  
 
 ************* Deployment commands *****************  
 kubectl apply -f .\3-deployment\solution\1.yaml  
 kubectl get pods  
 kubectl apply -f .\3-deployment\solution\2.yaml
 kubectl get pods  
 kubectl rollout status deployment/front-end  
 kubectl describe deployment/front-end  
 kubectl get deployments  
 
 ******************* Service Commands ****************  
 kubectl apply -f .\4-service\solution\1.yaml  
 kubectl apply -f .\4-service\solution\2.yaml  
 kubectl get services  
 
 ******************* Config Map commands ******************   
 kubectl create configmap front-end-config --from-file=5-configmaps/default.conf  
 kubectl apply -f .\3-deployment\solution\3.yaml  
 kubectl get pods  
 kubectl logs back-end-74948d5f7-npxz5  
 
 ************ Secrets Commands ************************  
 kubectl apply -f .\6-secrets\app-secret.yaml  
 kubectl apply -f .\3-deployment\solution\4.yaml  
 
 ***** deployment commands ********************  
 kubectl rollout history deployment/back-end  
 
 ****** out put format of deployment commands ************  
 kubectl get deployment front-end -o yaml  
 kubectl get deployment front-end -o json   
