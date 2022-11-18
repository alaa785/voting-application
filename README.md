# voting-application
Installing minikube with Vagrant and Ansible:
Clone vagrant-minikube directory to your working directory, then run vagrant upn & run vagrant ssh
copy or clone vot-app directory inside minikube instance & run kubectl -f vote-app/catvsdogs
check if the service is there : kubectl get services
after that run the following command : minikube service "vote/result" --url
hit vote/result URL: curl http://$(minikube ip):port_no  
secret object use to encode both of db_usr & db_pass
HPA used for vote auto-scaling.
