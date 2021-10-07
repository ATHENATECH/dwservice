# dwservice
Le service d'assistance technique a besoin de prendre la main distance pour vous aider à résoudre un problème technique. Nous vous donnerons quelque commande de serveur Linux pour fournir la prise en main aux supports.

L'application utilisé pour la prise en main à distance est DWService.  Choisis pour sa compatibilité sur des serveur Linux ne disposant pas d'interface graphique. Certain de nos produits disposent de cette application, comme DATASAVE ou DATASELF.

Pour lancer cette application,  saisissez sur votre serveur, en ligne de commande, "sudo sav-start". L'application DWService se lance et vous fournie un identifiant et un mot de passe à communiquer au support pour la prise en main à distance. Le support utilisera ses identifiant sur le site de DWService pour accéder aux terminal de votre serveur. Vous pouvez couper à tout moment la connexion de la prise en main à distance, il suffit d'utiliser le raccourcie clavier CTRL+C. 

Si jamais, vous avez changer de terminal ou mis l'application en arrière plan. Vous pouvez coupé la connexion de la prise en main à distance en utilisant la commande sav-stop. sav-end pour les anciennes version. Un message fin de transmission apparaît pour confirmer l’arrêt du service DWService.


Si DWService n'est pas présent sur votre serveur Linux, vous pouvez utilisez la commande suivante :
wget https://raw.githubusercontent.com/ATHENATECH/dwservice/main/dwservice.sh
pour télécharger le script qui va télécharger DWService, mettre en place les commande cité précédement et lancer DWService. Pour ce faire, donnez les droit d'exécution au script en saisissant "sudo chmod +x dwservice.sh. Puis inscrivez sudo ./dwservice.sh pour l'exécuter.

Pour raison de sécurité, le DWService, mis en place par notre script, ne s'exécutera pas au démarrage de votre serveur. Nous préférons laisser l'administrateur choisir le moment pour donner la prise en main à distance à nos supports techniques.  

Exemple de commande :

sudo sav-start

sudo sav-stop

sudo sav-end

wget https://raw.githubusercontent.com/ATHENATECH/dwservice/main/dwservice.sh

sudo chmod +x dwservice.sh

sudo ./dwservice.sh


Plus d'info sur DWService : https://www.dwservice.net/fr/home.html
