#  NUCLEAR HAMSTER PROJECT

Version Rouge :
![image](https://github.com/Nebrium/ProjetNH/assets/127872260/338b53e2-8498-4fe3-b1be-aceee29f30c0)

Version Bleue
![image](https://github.com/Nebrium/ProjetNH/assets/127872260/4b131220-34a2-4af2-be85-29369d8342e9)


Ceci est un simulateur d'attaque par rançongiciel. Elle simule l'ouverture d'une fenêtre faisant croire à l'utilisateur qu'il vient d'être attaqué par un rançongiciel.

Aucune donnée n'est chiffrée


#    Mode d'emploi : À lire avant de lancer le script

Les variables suivantes sont à renseigner avant le script :
- $NHVersion = Mettre RED pour la version rouge ou Blue pour la version bleue
- $AutoDesarmFolder = Chemin vers le répertoire local de désamorçage
- $AutoDesarmShare = Chemin vers le partage de désamorçage
- $LeftDateLimitTime = Réglage compteur de gauche
- $RightDateLimitTime = Réglage compteur de droite
- $KillTime = Durée d'exécution maximale du script
- $NoScriptTime = Date à partir de laquelle le script ne pourra plus s'ouvrir
- $KeyToClose = Touche pour fermer l'application en plus de la touche CTRL, par défaut "N"


Il existe 2 possibilités pour lancer le script :
- Lancer le script directement depuis une tâche planifiée avec la commande powershell.exe ./Ransomware.ps1
- Convertir le PS1 en exe avec PS2EXE /!\ Les antivirus bloqueront l'EXE /!\

Le script dispose d'une protection contre la fermeture. Alt + F4 ou Echap ne fonctionnent pas. Pour le fermer, il faut appuyer simultanément sur CTRL + la touche définie dans la variable $KeyToClose (N par défaut)

Il existe également un système d'auto-fermeture. Pour cela, il suffit d'indiquer un répertoire dans la variable $AutoDesarmFolder ou $AutoDesarmShare, dès que vous placez un fichier à l'intérieur, l'application se fermera.
