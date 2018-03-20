===== INFORMATIONS =====
Auteur : David Feng
Date : 07/03/18


===== Instructions =====
1. Télécharger et installer xampp
2. Télécharger et importer la base de données : FengyJobBdd
3. Télécharger le dossier FengyJob de github et l'importer dans xampp/htdocs/


===== TroubleShooting =====
10:20:52  [Apache] 	Problem detected!
10:20:52  [Apache] 	Port 443 in use by ""C:\Program Files (x86)\VMware\VMware Workstation\vmware-hostd.exe" -u "C:\ProgramData\VMware\hostd\config.xml"" with PID 7996!
10:20:52  [Apache] 	Apache WILL NOT start without the configured ports free!
10:20:52  [Apache] 	You need to uninstall/disable/reconfigure the blocking application
10:20:52  [Apache] 	or reconfigure Apache and the Control Panel to listen on a different port

1. Ouvrir le fichier httpd-ssl.conf dans apache\conf\extra
2. Rechercher la ligne avec "Listen 443"
3. Modifier le port comme vous le souhaitiez. Ici, j'ai utilisé le port 4430
4. Remplacer tous les "443" par "4430" dans le reste du fichier
5. Sauvegarder le fichier