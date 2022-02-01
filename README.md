# Kubernetes

Kubernetes Manifests para criação do cluster com os seguintes containers:

- Postgres container;
- Microservice Kotlin [link](https://github.com/adrmarciao/account-hexa-service-kotlin);
- Microservice Java (Em desenvolvimento);
- Mensageria usando Kafka (Em desenvolvimento);

Obs: Por ser um cluster com fins didáticos alguns pontos não foram levados em consideração:

 - Foi usado o namespace default
 - Namespace (dev/homo/prod)
 - Kind **Secret**, usado como uma minima proteção para adicionar password ou chaves, 
mas o ideal é usar um solução de vault presente em cloud services;

## Configuração

 - Instalar [Docker](https://www.docker.com/);
 - Instalar [MicroK8S](https://microk8s.io/);
 - Instalar [Git](https://www.docker.com/);
 - Clonar projeto;
 - Configurar Docker para aceitar kubernates, caso seja executado pelo windows;
 - Executar "kubectl apply -f ."
 - Executar "kubectl get all" e verificar se todos os service/pods estão sendo executados;
