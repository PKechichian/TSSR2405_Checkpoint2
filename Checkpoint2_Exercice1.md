## Exercice 1

#### Question 1.1

Le résultat d'un ping entre le serveur et le client renvoie une erreur car l'adresse IP du client (172.16.**100**.50) n'est pas sur le même sous-réseau que le serveur (172.16.**10**.10).

![pingServerClient](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-1.pingServCLI.png)

Ci-dessous la configuration IPv4 sur le client pour que le ping fonctionne :

![configCLI](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-1.configCLI.png)

Et le ping fonctionnel :

![pingServerClient](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-1.pingServCLIOK.png)

---

#### Question 1.2

Le serveur trouve le client par son nom grâce à l'adresse IPv6

![pingServerClientviaNom](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-2.pingAvecNom.png)

---

#### Question 1.3

Après désactivation du protocole IPv6, voici le résultat d'un ping du serveur vers le client.

Le ping fonctionne car le DNS a été configuré précédemment pour ma part, en ajoutant un hôte à la zone de recherche "SWEETCAKES" déjà existante.

Résultat ping :

![pingServerClient](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-3.pingAvecNomOK.png)

Configuration DNS :

![configDNS](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-3.configDNS.png)

---

#### Question 1.4

Le DHCP étant déjà configuré sur le serveur, il suffit de modifier les paramètres IPv4 du client pour qu'il obtienne une adresse IP automatiquement.

![configDNS](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-4.IPauto.png)

---

#### Question 1.5

Le client ne récupère pas la première adresse de la plage car les adresses 172.16.10.1 à 172.16.10.19 sont exclues de la ditribution par le DHCP.

![configDHCP](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-5.DHCP.png)

IP du client :

![IPclientDHCP](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-5.IPclient.png)

---

#### Question 1.6

Pour permettre au client d'avoir l'adresse 172.16.10.15, il faut modifier les zones d'exclusions dans le DHCP

![modifDHCP](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-6.modifDHCP.png)

---

#### Question 1.7

L'intérêt de passer en IPv6 serait de ne pas avoir à gérer de DHCP.
Mais le DHCP n'est pas obsolète pour autant, car il permet d'avoir une gestion pour précise du réseau.
Il permet de créer des plages comme pour IPv4.

