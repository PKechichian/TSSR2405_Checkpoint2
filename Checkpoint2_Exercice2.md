## Création d'un dossier partagé entre le serveur et le client

#### Q2.1

![DossierpartagéScript](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q2.sharedfolder1.png)

![DossierpartagéScript](https://github.com/PKechichian/TSSR2405_Checkpoint2/blob/main/Annexes/Q2.sharedfolder.png)

#### Q2.2

- Il ne se passe rien à l'éxécution du script (erreur)

- Il faut modifier le chemin du fichier pour "C:\Scripts\AddLocalUsers.ps1"

#### Q2.3  

L'option `-verb RunAS` sert à exécuter le script en tant qu'un autre utilisateur, ici Administrateur

#### Q2.4

L'option `-WindowsStyle -Maximized` sert à exécuter le script dans une nouvelle fenêtre maximizée

#### Q2.5

Le premier utilisateur ne s'affiche pas car il est mentionné dans la fonction `Import-Csv` l'option "-skip 2", donc ne prend pas en compte les 2 premières lignes (Entêtes + premier utilisateur)

#### Q2.6

Le champs Description n'est pas pris en compte car il n'est pas lié au champs dans la variable $UserInfo (ligne 39). 

#### Q2.7

Enlever les chanps inutiles dans la définition de la variable $Users (ligne 27)

#### Q2.8

Modifier le Write-Host (ligne 50) en `WriteHost "L'utilisateur $Prenom $Nom a été crée avec le mot de passe $pass" -ForegroundColor Green`

#### Q2.9

#### Q2.10

Rajouter un Write-Host sous le If de vérification

#### Q2.11

Manque un "s" à "Utilisateur" dans la dénomination -Group (ligne 51)

#### Q2.12

Créer la variable $Name = "$Prenom.$Nom" et remplacer dans le script

#### Q2.13

Changer PasswordNeverExpires (ligne 47) de $false à $true

#### Q2.14

Changer la variable $length de 6 à 12 (ligne 3)

#### Q2.15

Remplacer la ligne Start-Sleep par `Read-Host -Prompt "Appuyer sur Entrée pour continuer"`

#### Q2.16

`ManageAccentsAndCapitalLetters` permet de formatter les accents et les lettres majuscules pour uniformiser le texte, par exemple le ö du deuxième utilisateur
