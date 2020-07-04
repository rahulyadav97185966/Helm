# Helm
Helm is basically similar to the template in openshift


As I discuss Helm does same work like a template.
As We require deploymeny,service, pods, pv,pvc to run a complete application, in kubernetes we have to run these things separately
to overcome these the helm is usefull as it gives the chart which is known as Helm Chart which is available in hub of Helm.
Helm is widely used as it more functional.
  
     kubectl get nodes
    2  curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3
    3  chmod 700 get_helm.sh
    4  ./get_helm.sh
    5  kubectl get all
    6  helm repo add bitnami https://charts.bitnami.com/bitnami
    7  kubectl get all
    master $ history
    1  kubectl get nodes
    2  curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3
    3  chmod 700 get_helm.sh
    4  ./get_helm.sh
    5  kubectl get all
    6  helm repo add bitnami https://charts.bitnami.com/bitnami
    7  kubectl get all
    8  helm repo add bitnami https://charts.bitnami.com/bitnami
    9  helm install my-release bitnami/apache
    10  kubectl get all
     11  kubectl get pods
     12  kubectl get pods -w
     13  kubectl describe my-release-apache-7b4fc96476-qprqc
     14  kubectl describe deployment deployment.apps/my-release-apache
     15  kubectl describe deployment apps/my-release-apache
     16  kubectl describe apps/my-release-apache
     17  kubectl get all
     18  kubectl get al
     19  kubectl get all
     20  kubectl edit svc service/my-release-apache
     21  kubectl edit service service/my-release-apache
     22  kubectl edit service my-release-apache : just change loadbalancer to nodeport to access it outside of the cluster
     23  kubectl get all
     24  curl 10.104.240.44
