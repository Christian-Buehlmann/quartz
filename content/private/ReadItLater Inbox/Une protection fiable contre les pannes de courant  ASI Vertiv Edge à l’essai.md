[[ReadItLater]] [[Article]]

# [Une protection fiable contre les pannes de courant ? ASI Vertiv Edge à l’essai](https://www.digitec.ch/fr/page/une-protection-fiable-contre-les-pannes-de-courant-asi-vertiv-edge-a-lessai-25120)

![Martin Jud](https://www.digitec.ch/im/Files/3/9/8/9/8/5/2/7/joa.png?impolicy=PictureComponent&resizeWidth=36)

Si le fusible saute ou que l’électricité est coupée, il y a un risque de perte de données. Une alimentation sans interruption (ASI) permet de remédier à ce problème. J’ai testé un Vertiv Edge-750IMT et je l’ai apprécié à l’exception d’une chose.

Si vous souhaitez protéger votre serveur ou votre [Network Attached Storage (NAS)](https://www.digitec.ch/fr/page/migration-de-mon-nas-longue-vie-a-boba-fett-11466), ou un autre ordinateur contre la perte de données non enregistrées en cas de panne de courant, utilisez une alimentation sans interruption (ASI). Au lieu d’un raccordement direct à une prise électrique, l’électricité est fournie par l’onduleur qui possède une batterie intégrée qu’il utilise en cas de panne de courant. Cela permet bien sûr de protéger d’autres appareils contre les interruptions et de continuer à les alimenter en électricité. Si vous avez votre propre [serveur Plex](https://www.digitec.ch/fr/page/configurer-un-serveur-plex-11636), vous pourriez le raccorder, ainsi que le routeur et le téléviseur, à l’ASI et continuer à regarder des films pendant des minutes, voire des heures, selon la capacité de la batterie.

Dans mon ménage, une ASI pourrait convenir non seulement pour la télévision, mais aussi pour mon [installation de culture du cannabis](https://www.galaxus.ch/fr/page/une-installation-pour-cultiver-du-cannabis-chez-soi-compte-rendu-tinus-grow-episode-1-18052), qui fonctionne désormais avec des [LED](https://www.galaxus.ch/fr/s4/product/lumatek-zeus-600-w-pro-29-molj-culture-dinterieur-accessoires-21286962). Toutefois, je teste (pour l’instant) l’objectif primaire avec le PC et le NAS. Enfin, je veux savoir quels appareils peuvent établir une connexion de données avec l’ASI en plus d’une connexion électrique. En effet, cela permet d’éteindre automatiquement un appareil en cas de panne de courant après un temps prédéfini.

L’ASI utilisé dans ce test m’a été fournie par le fabricant. Les collègues du service des achats en ont parlé avec enthousiasme et ont dit que nous n’avions pas la marque Vertiv depuis longtemps dans notre boutique. Cela a éveillé ma curiosité, je suis impatient de découvrir le Vertiv Edge-750IMT avec une puissance nominale de 675 watts (750 voltampères) :

![Vertiv EDGE UPS 750VA/675W Tour IntelliSlot port (750 VA, 675 W, Line-interactive (classe de protection 5))](https://www.digitec.ch/im/Files/3/9/0/5/6/6/2/1/fe327928-6fb6-4314-97c9-f4426d717a4f.jpg?impolicy=ProductTileImage&resizeWidth=200&resizeHeight=200&cropWidth=200&cropHeight=200)

[](https://www.digitec.ch/fr/product/vertiv-edge-ups-750va675w-tour-intellislot-port-750-va-675-w-line-interactive-classe-de-protection-5-14044636)

En plus des prises, l’ASI dispose d’un port USB et d’un compartiment d’extension pour cartes supplémentaires, le port IntelliSlot. Afin d’obtenir des possibilités de connexion étendues, plus précisément un port RJ45 en plus du port USB, j’ai demandé une carte Vertiv Liebert Intellislot Elle met non seulement mon ASI en réseau, mais elle permet aussi d’utiliser le protocole SNMP (Simple Network Management Protocol). L’installation de la carte se fait en un clin d’œil, puisqu’il suffit de retirer un cache à l’arrière de l’ASI et de visser deux fois après l’avoir insérée.

![Vertiv IS-UNITY-SNMP](https://www.digitec.ch/im/Files/2/2/1/5/0/5/6/6/481585.jpg?impolicy=ProductTileImage&resizeWidth=200&resizeHeight=200&cropWidth=200&cropHeight=200)

[](https://www.digitec.ch/fr/product/vertiv-is-unity-snmp-accessoires-asi-10209413)

La série Edge existe d’ailleurs en plusieurs variantes, aussi bien avec différentes puissances nominales qu’en différents formats. Outre la mini-tour présentée dans ce test, le produit est également disponible dans un design compact de montage en rack 1HE ou en rack 2HE ou 3HE pour les systèmes de serveurs.

## Design, connexions et caractéristiques techniques

L’extérieur du Vertiv Edge-750IMT fait penser à un boîtier NAS surdimensionné. Il mesure 14,5 centimètres de large, 37 de long et 22 de haut et pèse 11 kilogrammes. La façade comporte deux LED d’état avec les mentions « Run » et « Alarm », un écran LCD et quatre touches de commande. Les informations, telles que l’utilisation actuelle ou l’état de la batterie, ainsi que toutes les options de l’appareil, peuvent être lues et réglées directement sur l’appareil.

[![Utilisable même la nuit ou dans les endroits sombres : écran avec rétroéclairage.](https://www.digitec.ch/im/Files/6/9/9/5/7/8/7/8/Vertiv_Edge_750-IMT_IMG12345_judma.jpg?impolicy=PictureComponent&resizeWidth=992&resizeHeight=744)](https://static.digitecgalaxus.ch/Files/6/9/9/5/7/8/7/8/Vertiv_Edge_750-IMT_IMG12345_judma.jpg)

Utilisable même la nuit ou dans les endroits sombres : écran avec rétroéclairage.

La deuxième possibilité d’utilisation est une interface web à laquelle vous pouvez accéder via un navigateur Internet en entrant l’adresse IP. Toutefois, cela n’est disponible que si vous installez, comme moi, une carte d’extension correspondante. Les fonctions avancées de la carte (serveur SNMP) ne peuvent pas être configurées directement sur l’appareil, mais uniquement via l’interface web. Vous pouvez voir la carte avec connexion réseau sur l’image suivante en haut à droite.

[![L’arrière de l’ASI.](https://www.digitec.ch/im/Files/6/9/9/5/8/5/4/9/Vertiv_Edge_750-IMT_DSC8933_judma.jpg?impolicy=PictureComponent&resizeWidth=992&resizeHeight=1377)](https://static.digitecgalaxus.ch/Files/6/9/9/5/8/5/4/9/Vertiv_Edge_750-IMT_DSC8933_judma.jpg)

L’arrière de l’ASI.

En haut à gauche se trouvent un port d’arrêt d’urgence (Emergency Power Off, en abrégé EPO) et un port USB, en dessous duquel on peut voir le ventilateur. Il est généralement très silencieux, sauf en cas de panne de courant ou de chargement de la batterie. L’alimentation électrique est assurée par une prise d’entrée (type C14) avec disjoncteur de circuit d’entrée et cinq prises de sortie de type C13.

Comme vous pouvez le voir, trois des prises sont noires et deux sont grises. Vous connectez aux prises noires tous les appareils critiques, comme le routeur, un PC ou un serveur, c’est-à-dire ceux qui doivent toujours être alimentés. Les grises permettent de raccorder des imprimantes et autres, tout ce qui peut rester sans courant en cas d’urgence. Les connexions grises peuvent être programmées, contrairement aux noires. Il est par exemple possible de régler une désactivation en cas de risque de surcharge de la batterie ou de définir des seuils pour la désactivation et l’activation.

Avec cet onduleur, vos appareils peuvent consommer jusqu’à 675 watts au total. En cas de panne de courant, l’appareil a besoin d’un temps de commutation de quatre à six millisecondes et fournit ensuite du courant via deux batteries de 9 ampères-heures. Le rendement de ce modèle devrait être de 95 % et le facteur de puissance (power factor) de 0,9. Les modules de batterie peuvent être remplacés.

## Connexion d’appareils

Un câble d’alimentation pour la prise d’entrée ainsi qu’un câble USB sont fournis avec l’ASI. Pour brancher des appareils, je me suis procuré les câbles d’alimentation C14 suivants :

![Secomp C13 à C14 (1.80 m)](https://www.digitec.ch/im/Files/2/1/3/7/9/3/5/4/19991515_a_102.jpg?impolicy=ProductTileImage&resizeWidth=200&resizeHeight=200&cropWidth=200&cropHeight=200)

[](https://www.digitec.ch/fr/product/secomp-c13-a-c14-180-m-cable-dalimentation-5779286)

![Furber T13 — C14 (0.30 m)](https://www.digitec.ch/im/Files/6/6/1/0/1/3/7/5/229884111_xxl3.jpg?impolicy=ProductTileImage&resizeWidth=200&resizeHeight=200&cropWidth=200&cropHeight=200)

[](https://www.digitec.ch/fr/product/furber-t13-c14-030-m-cable-dalimentation-21562447)

Je commence par alimenter l’ASI, et son ventilateur se met à faire du bruit comme une imprimante laser qui démarre. Il ne le fait que lorsque l’appareil est en charge et que la batterie présente une capacité de charge inférieure à 90 %. Si je suis assis devant l’ASI, mon décibelmètre Testo 815 indique un volume sonore de 60 décibels. À trois mètres de distance, le niveau sonore est encore de 42 décibels. Comme l’ASI est déjà chargée à plus de 85 % après le déballage, l’épisode est terminé en relativement peu de temps. À partir d’un niveau de batterie de 90 %, le ventilateur, s’il existe, ne se fait plus entendre que faiblement. Il faut compter environ trois heures et demie pour une charge complète de 1,8 ampère-heure.

Une fois l’ASI sous tension, je connecte le modem et le routeur, un commutateur et le NAS.

## Commande sur l’appareil et via l’interface web

Le courant ne circule pas automatiquement après le branchement. Il faut d’abord l’activer dans les paramètres. Comme l’écran LCD est rétroéclairé, il est possible de le faire rapidement et intuitivement directement sur l’appareil, même dans l’obscurité. Je navigue dans le menu « Commande » et j’active l’alimentation sous « Marche/Arrêt ». L’ASI se met alors en marche et les appareils démarrent. Le ventilateur de l’ASI reste silencieux. Sur l’écran, je peux lire que 12 % de l’alimentation électrique sont utilisés. La capacité de la batterie en cas de panne de courant est alors estimée à 135 minutes.

Je trouve des indications plus précises sur l’utilisation dans l’interface web. 93 voltampères et 50 watts sont actuellement utilisés.

[![Interface web : paramètres de l’ASI](https://www.digitec.ch/im/Files/6/9/9/5/9/1/2/4/Vertiv_Weboberflaeche_1.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=727)](https://static.digitecgalaxus.ch/Files/6/9/9/5/9/1/2/4/Vertiv_Weboberflaeche_1.png)

Interface web : paramètres de l’ASI

L’interface web n’est certes pas une beauté, mais elle offre de manière logique toutes les informations détaillées sur l’entrée, la sortie et la batterie, ainsi que tous les réglages que je souhaite.

[![Interface web : paramètres de la carte supplémentaire SNMP](https://www.digitec.ch/im/Files/6/9/9/5/9/1/2/3/Vertiv_Weboberflaeche_2.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=921)](https://static.digitecgalaxus.ch/Files/6/9/9/5/9/1/2/3/Vertiv_Weboberflaeche_2.png)

Interface web : paramètres de la carte supplémentaire SNMP

Un onglet avec la désignation de l’ASI contient toutes les options pour l’appareil. Un deuxième onglet, intitulé « Communications », permet d’accéder aux options de la carte supplémentaire installée. Outre la configuration de SNMP (v1 Trap, v1/v2c Access ou v3 User), il est possible d’y effectuer, entre autres, des réglages réseau pour IPv4, IPv6 et LLDP. Il est possible de configurer jusqu’à dix utilisateurs pour l’utilisation de l’interface web. Il est également possible de recevoir des notifications par e-mail et SMS ou de mettre en place un service à distance.

## Connexion de données via USB et SNMP

Ce que je savais déjà avant de recevoir l’appareil, c’est que les NAS de Synology ne sont pas compatibles avec la connexion USB. Cela signifie que le NAS est certes alimenté en électricité, mais qu’il ne peut pas établir une connexion de données avec l’ASI. Sur le site du fabricant Synology, je trouve une [liste de compatibilité](https://www.synology.com/fr-fr/compatibility?search_by=category&category=upses&p=1&change_log_p=1) qui ne contient malheureusement aucun appareil de Vertiv. Ou pas encore, car Vertiv m’a fait savoir qu’elle étudiait la possibilité de faire certifier à l’avenir ses produits ASI par Synology.

Mis à part certains systèmes d’exploitation adaptés spécifiquement par les fabricants, avec lesquels il n’y a pas de compatibilité pour des raisons de licence, l’ASI fonctionne via USB avec Windows, Linux et macOS. Soit avec des moyens embarqués, soit en utilisant le logiciel [Vertiv Power Assist](https://www.vertiv.com/en-us/support/software-download/software/vertiv-power-assist-software-download/) (en anglais).

Je teste cela avec un PC Windows : je connecte le câble USB, j’installe le logiciel, je le lance et je me réjouis parce que tout fonctionne du premier coup et sans autre intervention.

[![La page d’aperçu du programme montre non seulement que tout fonctionne bien, mais aussi la charge actuelle et le temps restant ainsi estimé de la charge de la batterie.](https://www.digitec.ch/im/Files/6/9/8/5/3/0/2/5/Vertiv_Power_Assist_1_judma.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=734)](https://static.digitecgalaxus.ch/Files/6/9/8/5/3/0/2/5/Vertiv_Power_Assist_1_judma.png)

La page d’aperçu du programme montre non seulement que tout fonctionne bien, mais aussi la charge actuelle et le temps restant ainsi estimé de la charge de la batterie.

Le type de connexion peut être défini dans les paramètres du programme. Outre l’USB, le SNMP et un mode client sont disponibles. Ce dernier sert à se connecter à un autre appareil déjà relié à l’ASI. Si, comme dans mon cas, la connexion à l’ASI est établie, vous pouvez définir quand l’ordinateur doit être éteint automatiquement en cas de panne de courant. Cela peut se produire immédiatement, après un certain nombre de minutes, lorsque la charge de la batterie n’atteint pas une certaine limite de capacité ou lorsque le temps de fonctionnement restant estimé est inférieur à un certain temps résiduel.

[![Les conditions d’arrêt en cas de panne de courant.](https://www.digitec.ch/im/Files/6/9/8/5/3/0/2/7/Vertiv_Power_Assist_3_judma.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=734)](https://static.digitecgalaxus.ch/Files/6/9/8/5/3/0/2/7/Vertiv_Power_Assist_3_judma.png)

Les conditions d’arrêt en cas de panne de courant.

Si vous souhaitez que le programme vous informe des coupures de courant par e-mail, c’est également possible. Pour cela, il faut définir un serveur SMTP et les données d’accès correspondantes.

[![Une notification peut aussi être réglée directement sur l’ASI avec une carte supplémentaire. Néanmoins, il est pratique que le Vertiv Power Assist offre également cette possibilité.](https://www.digitec.ch/im/Files/6/9/8/5/3/0/2/9/Vertiv_Power_Assist_5_judma.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=734)](https://static.digitecgalaxus.ch/Files/6/9/8/5/3/0/2/9/Vertiv_Power_Assist_5_judma.png)

Une notification peut aussi être réglée directement sur l’ASI avec une carte supplémentaire. Néanmoins, il est pratique que le Vertiv Power Assist offre également cette possibilité.

### Une mauvaise idée : connecter une ASI Vertiv et un NAS Synology via SNMP

J’ai déjà mentionné le fait que l’ASI de Vertiv ne peut pas être connectée à un NAS Synology via USB en raison de l’absence de licence. Mais chez moi, cela ne fonctionne pas non plus via SNMP. Au moins, le serveur SNMP de la carte supplémentaire fonctionne en principe, car la connexion se fait sans problème lors d’un essai avec le logiciel Power-Assist sur l’ordinateur Windows.

Avant le test, je suis confiant à cause du NAS, car Vertiv fournit sur son site Internet des [fichiers MIB SNMP](https://www.vertiv.com/de-emea/support/software-download/monitoring/management-information-bases-mibs-for-liebert-products/) (en anglais). Et parce que j’ai trouvé un [Synology DiskStation MIB Guide](https://global.download.synology.com/download/Document/Software/DeveloperGuide/Firmware/DSM/All/enu/Synology_DiskStation_MIB_Guide.pdf) (en anglais). MIB est l’abréviation de Management Information Bases, c’est-à-dire une base d’informations de gestion. Celle-ci se présente sous la forme de plusieurs fichiers dans un format texte. Vous pouvez l’imaginer comme une instruction ou une description de différents objets réseau, qui sert de pilote à l’appareil connecté à l’ASI. En bref, sans ces fichiers d’instructions, la connexion de données au NAS Synology ne fonctionne pas. Et malheureusement, la liste de sélection du champ de sélection MIB SNMP dans les paramètres du NAS ne contient que des partenaires ASI sous licence.

[![Pas de connexion sans MIB SNMP correcte, malheureusement.](https://www.digitec.ch/im/Files/6/9/9/5/9/1/4/8/Synology_USV_failed.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=738)](https://static.digitecgalaxus.ch/Files/6/9/9/5/9/1/4/8/Synology_USV_failed.png)

Pas de connexion sans MIB SNMP correcte, malheureusement.

Ce qui est également stupide, c’est que je n’ai pas regardé de plus près le guide MIB avant ce test. Il décrit entre autres comment les fichiers MIB sont convertis en fichiers Oidlib pour être ensuite importés. La conversion fonctionne parfaitement, mais j’échoue lors de l’importation, car je ne trouve pas l’indication permettant d’importer les données dans le système d’exploitation Synology « DiskStation Manager ». C’est alors seulement que je m’aperçois que les instructions datent de 2013, je n’en trouve pas de plus récentes. Et c’est ainsi que je perds patience, alors que je suis en train de bidouiller le serveur avec [Putty](https://www.putty.org/) (en anglais) et SSH.

Je décide donc d’abandonner la tentative. Le NAS reste connecté à l’ASI sans possibilité d’arrêt automatique en cas de panne de courant. Tant qu’une interruption ne dure pas plus de deux heures et quelques minutes et que je n’ai qu’une charge d’environ 50 watts, ce n’est pas tragique, car la batterie suffit alors.

## Quand l’électricité est coupée : voici comment le Vertiv Edge gère une panne d’alimentation décuplée

La LED Run mentionnée au début s’allume en vert en permanence dès que les appareils connectés sont alimentés. La LED d’alarme clignote en rouge dès qu’il y a une surcharge ou une panne de courant. De plus, l’ASI émet une alarme, un bip que je peux entendre dans tout l’appartement. Si vous le souhaitez, vous pouvez la désactiver dans les options.

En raison d’une surcharge, l’appareil n’émet un bip qu’une seule fois pendant des semaines. Je connecte une [imprimante laser tout-en-un](https://www.digitec.ch/fr/s1/product/brother-mfc-9140cdn-laser-couleur-imprimante-446711). Elle ne consomme certes qu’une dizaine de watts à vide, mais elle est un véritable monstre dans les premières secondes qui suivent sa mise en marche, dépassant ainsi la puissance nominale de l’alimentation sans coupure. Cependant, après quelques secondes d’alerte, tout rentre dans l’ordre. Je décide néanmoins de ne plus brancher l’imprimante, et encore moins de faire des tests avec. Comme vous pouvez le constater, il faut toujours bien planifier vos connexions.

Je subis ma première panne de courant lorsque, après mes vacances d’automne, j’active une multiprise dans mon bureau, dans laquelle sont branchés trop d’ordinateurs. Le fusible saute alors et l’ASI émet une alarme et passe en mode batterie. Les appareils qui y sont raccordés restent allumés.

Je provoque artificiellement dix autres coupures de courant, en les débranchant manuellement. Ce faisant, je reconnecte l’ordinateur Windows au port USB et je vérifie que l’arrêt automatique fonctionne. C’est ce qu’il fait, quel que soit le réglage ; c’est-à-dire juste après une panne de courant, après quelques minutes ou même lorsque la charge de la batterie est inférieure à la valeur prédéfinie. La commutation du courant fonctionne également sans problème à chaque fois.

Si vous voulez savoir combien de temps des batteries avec une capacité de 1,8 heure-ampère fournissent du courant à différentes charges, vous pouvez le découvrir en ligne avec le [Vertiv Runtime Tool](https://www.vertiv.com/fr-emea/assistance-technique/tools-applications/vertiv-ups-interactive-runtime-tools/vertiv-edge-1ph-ups/). Choisissez le modèle « EDGE-750IMT » et c’est parti. Si je raccordais mon serveur Plex, mon routeur et mon [TV](https://www.digitec.ch/fr/s1/product/samsung-qe85qn95a-4k-neoqled-va-2021-85-tv-14894606) à l’ASI comme mentionné au début, la consommation électrique atteindrait 210 watts. Je pourrais ainsi regarder la télévision pendant 30 minutes. Si la lumière LED de mes plants de cannabis était raccordée à l’ASI, que j’alimente en réduisant la puissance à 450 watts, une panne de courant ne devrait pas durer plus de onze minutes.

## Conclusion : une bonne ASI avec une protection irréprochable contre les pannes de courant et un potentiel de connexion extensible

Avec l’Edge-750IMT, Vertiv propose une alimentation sans interruption facile à utiliser pour des novices en matière d’ASI comme moi. Elle a surmonté toutes les pannes de courant sans problème et a toujours fourni du courant aux appareils qui y sont connectés. L’installation est simple et l’écran LCD rétroéclairé permet d’être informé et d’accéder rapidement à toutes les options.

Un petit bémol : jusqu’à présent, Vertiv n’a pas obtenu de licence auprès de Synology, c’est pourquoi la connexion de données à mon NAS est possible. Mais il faut aussi que le courant soit coupé pendant plus de deux heures, car c’est le temps que dure la batterie lorsque j’ai le serveur de stockage en réseau, le routeur, un commutateur et le modem connectés.

Concernant le prix : à mon avis, les cartes supplémentaires devraient coûter moins cher. Près de la moitié du prix de l’ASI est trop élevé pour une connexion RJ45 et un serveur SNMP, même avec la valeur ajoutée d’une interface web. Dommage que l’appareil ne soit pas équipé d’origine d’un port réseau en plus du port USB. En revanche, je ne trouve pas le prix de l’ASI proprement dit trop élevé, car il se situe dans la moyenne par rapport aux appareils ayant une puissance nominale et une capacité de batterie similaires.

Cet article plaît à 36 personne(s)

---

![User Avatar](https://www.digitec.ch/im/Files/3/9/8/9/8/5/2/7/joa.png?impolicy=PictureComponent&resizeWidth=96)

![User Avatar](https://www.digitec.ch/im/Files/3/9/8/9/8/5/2/7/joa.png?impolicy=PictureComponent&resizeWidth=48)

Le baiser quotidien de la muse stimule ma créativité. Si elle m’oublie, j’essaie de retrouver ma créativité en rêvant pour faire en sorte que mes rêves dévorent ma vie afin que la vie ne dévore mes rêves.

---

[Informatique](https://www.digitec.ch/fr/topic/1154)

Suivez les thèmes et restez informé dans les domaines qui vous intéressent.

---

[Réseau](https://www.digitec.ch/fr/topic/1418)

Suivez les thèmes et restez informé dans les domaines qui vous intéressent.

---

## Ces articles pourraient aussi vous intéresser

-   Skeleton Loader
    
    #### Skeleton Loader
    
-   Skeleton Loader
    
    #### Skeleton Loader
    
-   Skeleton Loader
    
    #### Skeleton Loader