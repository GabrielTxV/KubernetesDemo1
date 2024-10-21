#Demo Kubernetes/Docker project  
From https://www.youtube.com/watch?v=s_o8dwzRlu4  
Para iniciar, ''minikube deve estar rodando''  
```minikube start```     
Aplicar primeiramente config e secret antes dos deployments por referência     
``kubectl apply -f mongo-config.yaml`` // ``kubectl apply -f mongo-secret.yaml``    
Em seguida database e depois o webapp  
``kubectl apply -f mongo.yaml`` // ``kubectl apply -f webapp.yaml``  
Para checar funcionamento e ip - ``kubectl get all``  
``kubectl get xxx`` - para mais informações   
``minikube ip`` - revelar o ip do serviço - port está configurado no código (30100)  
``minikube service webapp-service`` - para acessar o serviço no navegador  
Parar o serviço/minikube - ``minikube stop`` 
