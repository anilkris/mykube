# mykube

- minikube start
- kubectl run mysql --image=mysql:5.5 --env MYSQL_ROOT_PASSWORD=root
- kubectl expose deployment mysql --port 3306
- kubectl run wordpress --image=wordpress --env WORDPRESS_DB_HOSTNAME=mysql --env WORDPRESS_DB_PASSWORD=root
- kubectl expose deployment wordpress --port 80 --type LoadBalancer
- kubectl get deployments
- kubectl get svc
- minikube ip
- run the url from minikube ip and port exposed by the service.
