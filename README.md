#  NUCLEAR HAMSTER PROJECT V2.0


Ceci est une simulateur d'attaque par rançongiciel. Elle simule l'ouverture d'une feanêtre faisant croire à l'utilisateur qu'il vient d'être attaqué par un rançongiciel.

Aucune donnée n'est chiffrée


#    Mode d'emploi : A lire avant de lancer le script


Il exsite 2 possibilités pour lancer le script :
    - Lancer le script directement depuis une tâche
      planifiée avec la commande 
      powershell.exe ./Ransomware.ps1
    - Convertir le PS1 en exe avec PS2EXE 
      /!\ Les antivirus bloqueront l'EXE /!\

Le script dispose d'une protection contre la fermeture. Alt + F4 ou Echap ne fonctionnent pas. Pour le fermer il faut appuyer simultanément sur CTRL + la touche définie dans la variable $KeyToClose (N par défaut)

Il existe également un système d'auto-fermeture. Pour cela il suffit d'indiquer un répertoire dans la variable $AutoDesarmFolder, dès que vous placez un fichier à l'intérieur, l'application se fermera.


#                 Historique des versions


Mai 2023
V1.0 : Release de la version Red

Août 2023
V2.0 : Ajout de la version Blue

