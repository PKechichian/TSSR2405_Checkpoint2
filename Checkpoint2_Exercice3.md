## Exercice 3

#### Q3.1

Il s'agit d'un switch, qui permet de faire la liaison physique entre les différents appareils.

#### Q3.2

Il s'agit d'un routeur, qui sert à router les paquets vers les adresses IP correctes

#### Q3.3

Il s'agit des noms des interfaces du routeur

#### Q3.4

/16 représente son masque de sous-réseau

#### Q3.5

Il s'agit de sa passerelle par défaut

#### Q3.6

| PC | Adresse réseau | Première adresse dispo | Dernière adresse dispo | Diffusion |
| --- | --- | --- | --- | --- |
| PC1 | 10.10.4.1 | 10.10.0.1 | 10.10.255.254 | 10.10.255.255 |
| PC2 | 10.11.80.2 | 10.11.0.1 | 10.11.255.254 | 10.11.255.255 |
| PC5 | 10.10.4.7 | 10.10.0.1 | 10.11.255.254 | 10.11.255.255 |

#### Q3.7

PC1, PC4 et PC5 peuvent communiquer entre eux, ainsi que PC2 et PC3

#### Q3.8

Tous les ordinateurs peuvent atteindre 172.16.5.0/24

#### Q3.9

Il n'y aura aucune incidence si on interverti les ports

#### Q3.10

Elles cont toutes avoir une adresse en 10.10.X.X

---

### Analyse de trames

#### Fichier 1

#### Q3.11

Source: 00:50:79:66:68:00 (00:50:79:66:68:00)

#### Q3.12

La communication a réussi entre 10.10.4.1 et 10.10.4.2

#### Q3.13

- Request : IP : 10.10.4.1 / MAC : 00:50:79:66:68:00
- Reply : IP : 10.10.4.2 / MAC : 00:50:79:66:68:03

#### Q3.14

Protocole ARP, qui sert à lié les IP aux adresses MAC

#### Q3.15

A sert de lien physique entre les machines, B sert de routeur

#### Fichier 2

#### Q3.16

10.10.80.3 initialise la communication

#### Q3.17

Le protocole encapsculé est ICMP, qui permet de ping

#### Q3.18

La communication n'a pas fonctionné car il n'y a pas de retour de l'IP contactée

#### Q3.19

Ne trouvant pas l'hôte 10.11.80.2, le ping repart vers la passerelle par défaut

#### Q3.20

A sert de lien physique, B sert de routeur

#### Fichier 3

#### Q3.21

- Source : 10.10.4.2
  
- Destination : 172.16.5.253

#### Q3.22

- Source: ca:01:da:d2:00:1c 

- Destination: ca:03:9e:ef:00:38 

#### Q3.23

Cette communication a été enregistré au niveau de R2



 
