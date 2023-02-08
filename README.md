# RealProject

Partie I : INSTALLATION DE OSMOCOM SUR LINUX 
I-Installation de osmocom 
1-Prérequis et Installation des dépendances
2-Configuration du HLR 
3-Configuration du mobile
4-Comportement du wireshark 
Conclusion 


Osmocom est un projet informatique comprenant toute une famille de projets de télécommunications mobile libres, parmi lesquels OsmocomBB, OsmocomGMR, OsmoSDR....
C'est un ensemble d'outils (tant logiciel que matériel) tel que Global System for Mobile Communications (GSM), DECT et d'autres moins connus (Terrestrial 
Trunked Radio (TETRA), GM).
			I-Installation de osmocom

				1- Prérequis et Installation des dépendances 
Comme pré-requis, on doit d'abord installer Synaptic qui est une interface graphique légère pour le système de gestion de paquets apt utilisé dans Debian, 
Ubuntu,Linux Mint et de nombreuses autres distributions basées sur Debian / Ubuntu.Ensuite on pourra intaller toutes les dépendances pour l'installation 
d'osmocom et ainsi cloner toutes les blibliothéques telles que libosmocore, libosmo-abis qui contient la bibliotheque d'interface A-bis.On a également 
libosmo-netif qui implémente le serveur de flux et les clients pour TCP, UDP, IPA; libosmo-sccp utilisée par les programmes OsmoBSC, OsmoMSC, OsmoSTP; 
libsmpp34. Enfin OsmoMGW, Osmocom Media Gateway, est une passerelle multimédia pour gérer le trafic du plan utilisateur (voix) dans les réseaux cellulaires. 
OsmoMGW prend en charge l'IETF MGCP (Media Gateway Control Protocol) pour le contrôle des agents d'appel, tels que ceux présents dans OsmoBSC et OsmoMSC . 
 				2-Configuration du HLR

Les requêtes HLR permettent de savoir si un numéro de téléphone mobile est valide avant de lui envoyer un SMS ou de l'appeler. Si le numéro est valide en
utilisant le HLR Lookup, le résultat nous permettra de connaître l’opérateur sur lequel le téléphone est enregistré.Le HLR constitue la base de données dans 
laquelle les informations suivantes sont vérifiées IMSI (International Mobile Subscriber Identity), identifiant unique de l'utilisateur et qui est stocké 
dans la carte SIM (connu uniquement de l’opérateur); l'IMEI définissant la Station Mobile utilisée, soit généralement, le téléphone mobile de l'utilisateur ;
MSISDN (Mobile Subscriber International ISDN Number), indiquant le numéro d'appel international via lequel l'utilisateur est joignable. Il est généralement 
unique pour un même IMSI (sauf cas particulier, ex : n° de Fax); les services souscrits par l'abonné, l'état des renvois d'appels, ...
				3-Configuration du mobile

Avant d'activer le mobile on doit d'abord executer le trx qui agit comme un pont entre l'émetteur-récepteur et les applications osmocomBB. Le mobile permet 
de se synchroniser sur la station de base du réseau local et il permet d'enregistrer un utulisateur .
				4-Comportement du wireshark

Le wireshark permet de résoudre les problémes de réseau, examine les problémes de sécurité, vérifie les applications réseaux, débogue les implementations
de protocole, apprend les rouages du protocole réseau. Il capture aussi les paquets et en fait un filtrage et une inspection. De plus Wireshark est utilisé
pour inspecter un programme suspect et analyser le flux de trafic sur le réseau ou résoudre des problémes liés au réseau.

