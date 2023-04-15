# 1- Explain the main difference between OSI model and TCP/IP model.
Le modèle OSI est un modèle conceptuel à 7 couches qui permet de décrire la communications entre ordinateurs, tandis que TCP/IP est un modèle pratique à 4 couches utilisé pour établir une connexion et communiquer via le réseau notamment internet.

# 2- Explain the application service layers and what happen when you write your url and click enter.
La couche Application est la 7ème couche du modèle OSI.
C'est là que les données sont préparées pour être utilisées par le logiciel de l'utilisateur, tel que le navigateur web ou les e-mails. 
C'est également la couche dans laquelle la communication est initiée avec le réseau lorsque des données sont envoyées depuis un appareil.
Cette couche est responsable des protocoles tels que HTTP, HTTPS et SMTP.

Une fois qu'on saisi l'URL dans un navigateur et qu'on appui sur "Entrée", le navigateur doit trouver le serveur avec lequel on veux communiquer.
Pour communiquer avec le serveur hébergeant le site web que nous avons demandé, il doit découvrir son adresse IP, ce qui permettra d'établir une connexion sur l'internet. 
Pour obtenir l'adresse IP, il existe des serveurs spécifiques appelés serveurs de noms de domaine (DNS) avec des adresses IP bien connues qui maintiennent des tables de noms de domaine et les adresses IP réelles des serveurs hébergeant leur contenu associé. 
Ainsi, le navigateur vérifie auprès d'un serveur DNS l'adresse IP réelle du site, puis adresse une seconde requête directement à l'adresse IP.
Le navigateur envoie une requête GET au serveur web en utilisant le protocole HTTP et attend une réponse, établissant ainsi une connexion bidirectionnelle entre l'ordinateur qui exécute le navigateur et le serveur web.
Côté serveur, les informations demandés seront collectées puis formatées en HTML avant d'être renvoyé au client.

# 3- Explain what is a domain name and the relation between the DNS and the @IP address.
Un nom de domaine est un nom lisibble et compréhensible par l'homme associé à une adresse ip moins compréhensible par l'homme. 
DNS est un service informatique qui associe des noms de domaine avec leurs adresses ip.

# 4- Explain the TCP interconnection between your local host and the server.
L'hôte local ou client envoie au serveur un paquet ou segment SYN (SYN signifie synchroniser) avec un numéro unique et aléatoire. Ce numéro garantit une transmission complète dans le bon ordre (sans doublons).
Quand le serveur reçoit le segment, il accepte la connexion en renvoyant un paquet SYN-ACK (ACK signifie acquittement) comprenant le numéro de séquence du client plus 1. Il transmet également son propre numéro de séquence au client.
Enfin, le client accuse réception du segment SYN-ACK en envoyant son propre paquet ACK, qui contient dans ce cas le numéro de séquence du serveur plus 1. 
La connexion étant ainsi établie, le client peut commencer à transférer des données au serveur.

# 5- How data transfer over internet (TCP Packet)
Lorsqu'elles sont transmises, les données sur Internet sont divisées en paquets plus petits d'environ 1 500 octets chacun.
Chaque paquet contient des informations sur l'adresse de l'expéditeur, l'adresse du destinataire, la place des données dans l'ensemble du message et comment l'ordinateur destinataire peut être sûr que les données sont arrivées intactes. 
