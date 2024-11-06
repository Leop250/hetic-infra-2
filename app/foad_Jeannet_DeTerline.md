nom et prenom:

Kylain Jeannet
Léopold Macquart de Terline

Utilité : ECS est un service qui permet de faire tourner des conteneurs Docker
Clsuter avce Fargate : Fargate est une option qui automatise la gestion des serveurs etr les MAJ

Le Load Balancer répartit le trafic entre les deux zones de disponibilité. Cela signifie que si un des conteneurs (ou même une zone entière) a un problème, le trafic peut être redirigé vers l'autre zone, garantissant que ton application reste accessible. (reverse proxi)

Amazon RDS les données sont stockées et accessibles par le backend.

Security group sont des pare-feu virtuels associés à les ressources AWS pour contrôler le trafic

VCP  est un environnement réseau privé dans lequel les ressources AWS seront déployées

CloudFront : Utilisé pour la distribution de contenu, afin d'optimiser l'accès aux utilisateurs, avec un cache près de l'utilisateur

Amazon S3 : Stockage d'objets pour des fichiers statiques comme des images ou des documents.

Public Subnet A et B : Ces sous-réseaux publics contiennent des ressources exposées à Internet.


