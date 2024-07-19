## Exercice 1

#### Question 1.1

Le résultat d'un ping entre le serveur et le client renvoie une erreur car l'adresse IP du client (172.16.**100**.50) n'est pas sur le même sous-réseau que le serveur (172.16.**10**.10).

![pingServerClient](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-1.pingServCLI.png)

Ci-dessous la configuration IPv4 sur le client pour que le ping fonctionne :

![configCLI](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-1.configCLI.png)

Et le ping fonctionnel :

![pingServerClient](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q1-1.pingServCLIOK.png)
