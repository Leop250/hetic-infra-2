nom et prenom:

Kylain Jeannet
Léopold Macquart de Terline


qustion 1 
Utilité : ECS est un service qui permet de faire tourner des conteneurs Docker
Clsuter avce Fargate : Fargate est une option qui automatise la gestion des serveurs etr les MAJ

Le Load Balancer répartit le trafic entre les deux zones de disponibilité. Cela signifie que si un des conteneurs (ou même une zone entière) a un problème, le trafic peut être redirigé vers l'autre zone, garantissant que ton application reste accessible. (reverse proxi)
Amazon RDS les données sont stockées et accessibles par le backend.
Security group sont des pare-feu virtuels associés à les ressources AWS pour contrôler le trafic
VCP  est un environnement réseau privé dans lequel les ressources AWS seront déployées
CloudFront : Utilisé pour la distribution de contenu, afin d'optimiser l'accès aux utilisateurs, avec un cache près de l'utilisateur
Amazon S3 : Stockage d'objets pour des fichiers statiques comme des images ou des documents.
Public Subnet A et B : Ces sous-réseaux publics contiennent des ressources exposées à Internet.


Question 2
le liens vers le ficier qui cointient le shemat https://excalidraw.com/#json=cTXQMBGPKhV6Md7rJhepO,Y3xVaHQ6rCbqvmX429wBoQ




question 3:
L'architecture que j'ai choisie repose sur des services AWS qui assurent la performance, la fiabilité et la maîtrise des coûts de l'application. J'ai opté pour ECS avec Fargate, qui gère automatiquement les conteneurs sans avoir besoin de gérer l'infrastructure sous-jacente. Cela permet une scalabilité dynamique, en ajustant automatiquement les ressources en fonction de la demande, ce qui évite de payer pour des ressources sous-utilisées. Le Load Balancer, combiné à plusieurs Zones de Disponibilité (AZ), garantit une haute disponibilité et une tolérance aux pannes, redirigeant le trafic vers une autre zone en cas de problème. J'ai également intégré VPC et des Security Groups pour sécuriser l'ensemble de l'architecture et limiter les risques d'intrusion, en isolant les ressources critiques du reste du réseau. Côté gestion des données, Amazon RDS pour les bases relationnelles et DynamoDB pour les besoins NoSQL permettent une gestion efficace des données, tandis que S3 assure un stockage sécurisé et durable des objets. Le modèle pay-as-you-go d'AWS permet d'optimiser les coûts, car on ne paie que pour ce qui est utilisé. Enfin, avec des outils comme CloudWatch pour la surveillance et ECR pour le stockage des images Docker, je peux gérer de manière proactive les ressources et automatiser les déploiements avec CodePipeline, assurant ainsi une mise à jour continue sans perturber le service. Cette architecture garantit donc une solution robuste, évolutive et sécurisée, tout en optimisant les coûts et en assurant une gestion simplifiée.



question bonus: 
Amazon Elastic Container Registry (ECR). Ce service permet de stocker, gérer et déployer les images Docker de manière sécurisée et intégrée avec AWS, ce qui facilite leur utilisation dans ECS avec Fargate.

