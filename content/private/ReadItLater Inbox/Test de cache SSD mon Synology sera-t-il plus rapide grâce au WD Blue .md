[[ReadItLater]] [[Article]]

# [Test de cache SSD: mon Synology sera-t-il plus rapide grâce au WD Blue ?](https://www.digitec.ch/fr/page/test-de-cache-ssd-mon-synology-sera-t-il-plus-rapide-grace-au-wd-blue--17912)

![Martin Jud](https://www.digitec.ch/im/Files/3/9/8/9/8/5/2/7/joa.png?impolicy=PictureComponent&resizeWidth=36)

Le cache SSD dans le NAS accélère le flux de données entre la RAM et le disque dur. En théorie, il donne un coup de pouce au stockage en réseau, un peu comme une chambre de postcombustion. En pratique, ses flammes ne s'embrasent pas toujours avec la même intensité.

Les quatre [disques durs Ironwolf 8 To](https://www.digitec.ch/fr/s1/product/seagate-ironwolf-8tb-35-cmr-festplatte-12243540) Seagate de mon [NAS DS918+ Synology](https://www.digitec.ch/fr/s1/product/synology-ds918-netzwerkspeicher-nas-6563618) ont un taux de transfert allant jusqu'à 210 Mo/s, soit 1,68 Gbit/s, ce qui, à première vue, peut facilement alimenter mon réseau gigabit. Cela étant, les disques durs et les disques SSD n'offrent des taux de transfert rapides que si, premièrement, la connexion de données est conçue à cet effet et, deuxièmement, les fichiers à livrer ne sont pas trop petits, plus de 128 Ko.

Au fait, je ne les sors pas de nulle part ces 128 Ko. C'est ce que montrent les tests, comme celui du SSD réalisé par mon collègue, [Kevin](https://www.digitec.ch/User/kevin-hofer-2663159) :

-   [](https://www.digitec.ch/fr/page/samsung-980-pro-le-nec-plus-ultra-des-ssd-avec-bus-pcie-40--17633)
    
    ![](https://www.digitec.ch/im/Files/3/8/2/3/2/3/9/7/teaser21.jpeg)
    
    Test de produit
    
    #### Samsung 980 Pro : le nec plus ultra des SSD avec bus PCIe 4.0 ?
    
    par Kevin Hofer
    

Comme le disque dur ou le SSD doit s'adapter lors de la copie de chaque nouveau fichier, de nombreux petits fichiers sont copiés beaucoup plus lentement que les gros. Néanmoins, les vitesses théoriques d'écriture et de lecture des SSD sont beaucoup plus élevées que celles des disques durs. Et c'est là que deux [WD Blue SN550 SSD](https://www.digitec.ch/fr/s1/product/wd-blue-sn550-500gb-m2-2280-ssd-12452317) entrent en jeu : sur la fiche technique, ces derniers peuvent atteindre une vitesse plus de dix fois supérieure à celle de mes disques durs NAS. Pour l'accès en lecture, il est de 19,2 Gbit/s, pour l'accès en écriture, de 14. Mais en théorie uniquement.

Pour obtenir plus de détail sur l'utilité du cache SSD en aparté de ce test, je vous invite à lire cet article :

-   [](https://www.digitec.ch/fr/page/mise-a-niveau-nas-a-quoi-sert-le-cache-ssd--16085)
    
    ![](https://www.digitec.ch/im/Files/3/4/7/8/6/2/4/1/DSC0480721.jpeg)
    
    Guide
    
    #### Mise à niveau NAS : à quoi sert le cache SSD ?
    
    par Martin Jud
    

En résumé, l'objectif du cache SSD en fonctionnement normal est de rendre une petite partie de l'ensemble des données stockées – la partie à laquelle on accède fréquemment – disponible plus rapidement. Le stockage en réseau utilise un algorithme LRU \[Least Recently Used, le moins récemment utilisé (NdT)\] pour déterminer les fichiers à mettre en cache.

## Préparation des tests : installation et configuration du cache

Mon NAS peut intégrer deux SSD, soit le minimum requis pour créer un cache en lecture-écriture sur un appareil Synology. On pourrait créer un cache avec un seul SSD, mais cela n'accélère pas les téléchargements vers l'appareil.

J'ai deux SSD WD Blue de 500 Go, installés en une minute, deux couvercles en plastique sur la partie inférieure du boîtier du NAS exposant les ports M.2 et facilitant l'installation.

À l'issue de cet article, si vous décidez de passer au cache SSD, consultez alors le guide du cache SSD de Synology pour des conseils et des recommandations supplémentaires sur la taille du cache, basés, entre autres, sur des statistiques d'accès de ces derniers jours.

[![Sur la base du transfert de données de ces derniers jours, le guide propose une recommandation sur la quantité de cache SSD à installer.](https://www.digitec.ch/im/Files/3/8/9/3/6/7/5/0/synology_ssd_cache_ratgeber.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=713)](https://static.digitecgalaxus.ch/Files/3/8/9/3/6/7/5/0/synology_ssd_cache_ratgeber.png)

Sur la base du transfert de données de ces derniers jours, le guide propose une recommandation sur la quantité de cache SSD à installer.

Dans mon cas, la taille recommandée de 4,6 To peut ne pas être correcte. Ces derniers jours, j'ai copié beaucoup plus de fichiers que d'habitude à des fins de test. Par conséquent, l'évaluation de Synology n'est réalisée qu'à des fins statistiques. J'espère que les résultats de mes tests me donneront une meilleure idée de la taille et de la rapidité des SSD dans mon cas, et que tout cela en vaut ne serait-ce que la peine.

Une fois les SSD installés et le stockage réseau redémarré, le cache peut être créé dans [DiskStation Manager](https://www.synology.com/de-de/dsm) comme suit :

**1.** ouvrir le gestionnaire de stockage (storage manager) ;

[![](https://www.digitec.ch/im/Files/3/8/9/3/7/4/8/6/synology_ssd_cache_erstellen.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=384)](https://static.digitecgalaxus.ch/Files/3/8/9/3/7/4/8/6/synology_ssd_cache_erstellen.png)

**2.** sélectionner l'élément de menu « SSD Cache » puis cliquer sur « Create » ;

**3.** suivre les instructions : sélectionner le mode cache (lecture seule ou cache en lecture/écriture), le volume et les SSD que vous souhaitez utiliser ainsi que les [types RAID](https://www.digitec.ch/fr/page/nasgeforscht-welcher-raid-typ-passt-zu-mir-11323). Pour moi, seul le RAID 1 fonctionne avec un cache en lecture-écriture, les RAID 5 et 6 restent grisés. L'assistant d'installation détecte automatiquement que rien d'autre n'est compatible avec mon RAID 10 NAS ;

[![](https://www.digitec.ch/im/Files/3/8/9/3/7/9/2/5/synology_ssd_cache_groesse.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=801)](https://static.digitecgalaxus.ch/Files/3/8/9/3/7/9/2/5/synology_ssd_cache_groesse.png)

**4.** à la dernière étape, sélectionner la taille de cache souhaitée. Une quantité inférieure au maximum n'a de sens que si vous avez également différents volumes entre lesquels vous souhaitez répartir l'espace du SSD.

L'intégration du cache SSD dans le système prend un peu plus d'une minute.

[![](https://www.digitec.ch/im/Files/3/8/9/3/8/0/2/0/synology_ssd_cache_healthy.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=592)](https://static.digitecgalaxus.ch/Files/3/8/9/3/8/0/2/0/synology_ssd_cache_healthy.png)

Je garderai un œil sur l'affichage de la taille du cache SSD précédent sur l'image ci-dessus lors des prochains tests. Le but de la manœuvre ? M'assurer que les données arrivent vraiment là où elles sont censées arriver. Maintenant, tout est prêt pour les tests. Ou presque tout du moins :

[![](https://www.digitec.ch/im/Files/3/8/9/4/1/9/8/6/synology_ssd_cache_skip.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=592)](https://static.digitecgalaxus.ch/Files/3/8/9/4/1/9/8/6/synology_ssd_cache_skip.png)

Après avoir créé un nouveau cache SSD, l'élément « Skip sequential I/O » se trouve sous l'onglet « Configure ». Cette option est correctement activée. Contrairement à la lecture ou à l'écriture mixte ou aléatoire, les accès I/O séquentiels – par exemple lors de la copie d'un gros fichier vidéo – avec cache SSD n'ont qu'un faible avantage en raison d'une augmentation de la vitesse. Pour cette raison, et surtout pour sauvegarder les SSD, les disques durs sont accessibles directement lors des opérations séquentielles quand cette option est activée. Pour cet article, cependant, j'ai désactivé l'élément de sorte que tout passe par le cache.

## Test cache SSD : transfert de données via Gigabit Ethernet et USB 3.0 (5 Gbit)

Comme mon réseau ne délivre qu'un gigabit par seconde, mais que je veux aussi montrer l'impact du cache sur une connectivité plus rapide, je procède à un test s'articulant autour de trois méthodes : avec le [SSD de Samsung](https://www.digitec.ch/fr/s1/product/samsung-portable-t5-1000gb-externe-ssd-6435475) externe connecté directement au port USB 3.0 du NAS, délivrant jusqu'à 5 Gbits/s, le transfert via Gigabit Ethernet et enfin la vitesse de copie interne.

Pour couvrir différents scénarios, j'ai choisi les quatre tests suivants pour déterminer la vitesse moyenne de téléchargement en amont et en aval, avec et sans cache SSD :

-   transfert de données d'un gros fichier vidéo ; version UHD de « Matrix Revolutions » en MKV avec 50,5 Go ;
-   transfert de nombreuses photos au format RAW ; 2215 fichiers ARW d'un Sony RX100, d'une taille moyenne de 19,8 Mo ;
-   transfert de nombreux fichiers JPG ; total de 2349 photos d'une taille moyenne de 4,4 Mo ;
-   transfert de nombreux petits fichiers ; 14 380 polices différentes au format TTF avec une moyenne de 59 Ko.

### Test des 50,5 Go avec film UHD

Pour s'échauffer, ainsi que pour sonder la vitesse moyenne maximale possible de la configuration actuelle, je commence les tests par un film UHD. Je télécharge 50,5 Go en amont et en aval. Selon la connexion et le sens de transfert, cela ne prend que 3 minutes 41 secondes ou jusqu'à 7 minutes 39 secondes par tentative.

En détail, le NAS (Network Attached Storage) fonctionne comme suit : les résultats pour le cache SSD sont en vert, les autres données de résultats, en Mo/s :

[![Ø Mo/s, barres de couleur verte = avec SSD Cache](https://www.digitec.ch/im/Files/3/8/9/7/1/1/6/2/synology_ssd_cache_test_mkv_new.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=1168)](https://static.digitecgalaxus.ch/Files/3/8/9/7/1/1/6/2/synology_ssd_cache_test_mkv_new.png)

Ø Mo/s, barres de couleur verte = avec SSD Cache

En mettant les résultats en relation, on remarque une augmentation de la vitesse avec le cache SSD lors de la copie d'un gros fichier de 50,5 Go :

| USB Download   (5 Gbps) | +12.86% | +26.1 MBps |
| --- | --- | --- |
| USB Upload   (5 Gbps) | +8.59% | +16.7 MBps |
| LAN Download   (1 Gbps) | +0.44% | +0.5 MBps |
| LAN Upload   (1 Gbps) | +0.44% | +0.5 MBps |
| Internal Copy | +47.05% | +74.9 MBps |

Lors du transfert de fichiers très volumineux, la copie interne bénéficie le plus du cache. Ça ne m'étonne guère. Cependant, je m'attendais à ce que l'augmentation de la vitesse soit beaucoup plus importante. Peut-être que le cache SSD est déjà plein ou que la température est trop élevée ? En tout cas, les 234,1 Mo/s, ou 1,87 Gbits/s, représentent une augmentation de 47,05 % par rapport au fonctionnement du disque dur.

Le SSD sur port USB permet d'obtenir un dixième de la vitesse de sortie. Le port LAN ne bénéficie pas du tout du cache. À 113 Mo/s, c'est tout simplement le maximum qui peut être atteint avec ma configuration réseau actuelle.

### Test 19,8 Mo avec données des photos RAW

Je vais serrer un peu la vis. 42,8 Go de données photographiques RAW d'une taille moyenne de 19,8 Mo sont envoyés en cours de route. Cela prend de 3 minutes 23 secondes à 9 minutes 6 secondes par passage.

Voici les résultats :

[![Ø Mo/s, barres de couleur verte = avec SSD Cache](https://www.digitec.ch/im/Files/3/8/9/7/1/1/5/8/synology_ssd_cache_test_arw_new.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=1168)](https://static.digitecgalaxus.ch/Files/3/8/9/7/1/1/5/8/synology_ssd_cache_test_arw_new.png)

Ø Mo/s, barres de couleur verte = avec SSD Cache

Augmentation de la vitesse avec cache SSD lors du transfert de fichiers d'une taille de 19,8 Mo :

| USB Download   (5 Gbps) | +12.25% | +23.5 MBps |
| --- | --- | --- |
| USB Upload   (5 Gbps) | +0.91% | +1.8 MBps |
| LAN Download   (1 Gbps) | +21.89% | +17.6 MBps |
| LAN Upload   (1 Gbps) | +4.80% | +3.9 MBps |
| Internal Copy | +57.88% | +79.7 MBps |

Par rapport au gros fichier MKV, la vitesse de transmission diminue d'environ 15 à 20 Mo/s. Mais maintenant, toutes les connexions tirent profit du cache. L'augmentation de plus de 20 % de la vitesse de téléchargement en réseau local me fait plaisir, car je charge souvent des données RAW directement depuis le stockage réseau dans Photoshop. Au niveau du stockage, on constate une augmentation de la vitesse de près de 5 %.

La copie via le port USB est deux fois moins efficace. En contrepartie, la copie interne avec cache SSD est très élevée et affiche un gain de près de 80 Mo/s.

### Test des 4,4 Mo avec fichiers JPG

Avec des fichiers JPG d'une taille moyenne de 4,4 Mo, je dis adieu aux vitesses supérieures à 200 Mo/s. Les 2349 fichiers, d'une taille totale de 10,1 Go, prennent entre 54 secondes et 3 minutes 21 secondes par test.

Résultats :

[![Ø Mo/s, barres de couleur verte = avec SSD Cache](https://www.digitec.ch/im/Files/3/8/9/7/1/1/6/0/synology_ssd_cache_test_jpg_new.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=1168)](https://static.digitecgalaxus.ch/Files/3/8/9/7/1/1/6/0/synology_ssd_cache_test_jpg_new.png)

Ø Mo/s, barres de couleur verte = avec SSD Cache

Augmentation de la vitesse avec cache SSD lors du transfert de fichiers d'une taille de 4,4 Mo :

| USB Download   (5 Gbps) | +49.25% | +52.7 MBps |
| --- | --- | --- |
| USB Upload   (5 Gbps) | +11.89% | +18.7 MBps |
| LAN Download   (1 Gbps) | +64.60% | +33.4 MBps |
| LAN Upload   (1 Gbps) | +22.18% | +12.0 MBps |
| Internal Copy | +122.31% | +105.8 MBps |

Des fichiers encore plus petits, un traitement encore plus lent et une vitesse encore plus élevée augmentent grâce au cache SSD. Pour les fichiers d'une taille de 4,4 Mo, il y a une augmentation substantielle de près de 50 et 65 % respectivement, surtout lors du téléchargement. Lors du téléchargement, mon réseau local est un peu plus rapide d'un cinquième. La copie interne pose un jalon avec une augmentation des performances de 122,31 %.

### Test 59 Ko avec 14 380 polices

De nombreux petits accès mettent les supports de stockage à mal. Donc un dossier de l'année 2010 contenant 14 380 fichiers TTF devrait tout à fait y parvenir. Attention NAS, tu vas morfler !

La taille totale de seulement 839 Mo semble relativement petite avant le test, mais un seul passage prend entre 57 secondes et 6 minutes 59 secondes.

Résultats :

[![Ø Mo/s, barres de couleur verte = avec SSD Cache](https://www.digitec.ch/im/Files/3/8/9/7/1/1/6/3/synology_ssd_cache_test_ttf_new.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=1168)](https://static.digitecgalaxus.ch/Files/3/8/9/7/1/1/6/3/synology_ssd_cache_test_ttf_new.png)

Ø Mo/s, barres de couleur verte = avec SSD Cache

Augmentation de la vitesse avec cache SSD lors du transfert de fichiers d'une taille de 59 Ko :

| USB Download   (5 Gbps) | +22.50% | +2.7 MBps |
| --- | --- | --- |
| USB Upload   (5 Gbps) | +11.97% | +1.4 MBps |
| LAN Download   (1 Gbps) | +9.09% | +0.3 MBps |
| LAN Upload   (1 Gbps) | +10.00% | +0.2 MBps |
| Internal Copy | +35.00% | +2.1 MBps |

Plus le fichier est petit, plus le transfert est lent et plus la vitesse augmente ? Non, ce n'est pas le cas. L'augmentation de la vitesse est plus importante avec des fichiers de 4,4 Mo qu'avec les polices de 59 Ko pour presque chaque connexion. Dans certains cas, elle est même considérable. Néanmoins, les polices bénéficient d'une postcombustion de 9 à 35 %.

Ce qui saute aux yeux, ce sont les vitesses terriblement basses des petits fichiers. Même avec le cache SSD, mon NAS n'est pas à la hauteur. Et en regardant les résultats avec Gigabit Ethernet, je me demande si je pourrais en tirer quelque chose avec d'autres appareils de réseau. Je n'arrive pas à me débarrasser du sentiment que le routeur, un commutateur ou la puce réseau de mon PC provoque un goulot d'étranglement.

Au fait : pour ce test, la copie interne relève du SSD connecté pour la première fois via USB.

### Vue d'ensemble : vitesse par connexion

Comme il peut être utile de voir les vitesses déterminées sous un angle différent, j'ai également trié les résultats par connexion. On obtient ainsi l'image suivante.

#### Transfert de fichiers USB (jusqu'à 5 Gbits/s)

[![Ø Mo/s, barres de couleur verte = avec SSD Cache](https://www.digitec.ch/im/Files/3/8/9/7/1/1/6/4/synology_ssd_cache_test_usb_new.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=1168)](https://static.digitecgalaxus.ch/Files/3/8/9/7/1/1/6/4/synology_ssd_cache_test_usb_new.png)

Ø Mo/s, barres de couleur verte = avec SSD Cache

Augmentation de la vitesse grâce au cache SSD avec une connexion de 5 Gbits :

| 50,5 GB Download | +12.86% | +26.1 MBps |
| --- | --- | --- |
| 50,5 GB Upload | +8.59% | +16.7 MBps |
| 19.8 MB Download | +12.25% | +23.5 MBps |
| 19.8 MB Upload | +0.91% | +1.8 MBps |
| 4.4 MB Download | +49.25% | +52.7 MBps |
| 4.4 MB Upload | +11.89% | +18.7 MBps |
| 59 KB Download | +22.50% | +2.7 MBps |
| 59 KB Upload | +11.97% | +1.4 MBps |

#### Transfert de fichiers LAN (jusqu'à 1 Gbit/s)

[![Ø Mo/s, barres de couleur verte = avec SSD Cache](https://www.digitec.ch/im/Files/3/8/9/7/1/1/6/1/synology_ssd_cache_test_lan_new.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=1168)](https://static.digitecgalaxus.ch/Files/3/8/9/7/1/1/6/1/synology_ssd_cache_test_lan_new.png)

Ø Mo/s, barres de couleur verte = avec SSD Cache

Augmentation de la vitesse grâce au cache SSD via Gigabit Ethernet :

| 50,5 GB Download | +0.44% | +0.5 MBps |
| --- | --- | --- |
| 50,5 GB Upload | +0.44% | +0.5 MBps |
| 19.8 MB Download | +21.89% | +17.6 MBps |
| 19.8 MB Upload | +4.80% | +3.9 MBps |
| 4.4 MB Download | +64.60% | +33.4 MBps |
| 4.4 MB Upload | +22.18% | +12.0 MBps |
| 59 KB Download | +9.09% | +0.3 MBps |
| 59 KB Upload | +10.00% | +0.2 MBps |

#### Copie interne

[![Ø Mo/s, barres de couleur verte = avec SSD Cache](https://www.digitec.ch/im/Files/3/8/9/7/1/1/5/9/synology_ssd_cache_test_internal_new.png?impolicy=PictureComponent&resizeWidth=992&resizeHeight=1168)](https://static.digitecgalaxus.ch/Files/3/8/9/7/1/1/5/9/synology_ssd_cache_test_internal_new.png)

Ø Mo/s, barres de couleur verte = avec SSD Cache

Augmentation de la vitesse grâce au cache SSD lors de copie interne :

| 50,5 GB Copy | +47.05% | +74.9 MBps |
| --- | --- | --- |
| 19.8 MB Copy | +57.88% | +79.7 MBps |
| 4.4 MB Copy | +122.31% | +105.8 MBps |
| 59 KB Copy | +35.00% | +2.1 MBps |

## Conclusion : le cache SSD peut être recommandé sous condition

Après ces tests, il m'apparaît clairement que je ne tirerai bénéfice du cache SSD que rarement. Les raisons ? Mon NAS, qui diffuse principalement des films en streaming, la connexion par Gigabit Ethernet, dont la plus grande augmentation de performance avec le cache est de 64,6 %, et ce, lors du téléchargement de fichiers d'une taille de 4,4 Mo. Cela concerne par exemple les fichiers JPG ou MP3, à partir desquels on peut ensuite télécharger environ 19 morceaux par seconde avec cache SSD au lieu de 12 jusqu'à présent. En traitant des données de photos RAW d'environ 20 Mo, le téléchargement n'est que d'un cinquième plus rapide. Avec les petits dossiers, d'un dixième seulement.

Dans l'ensemble, je pense qu'il vaut mieux mettre de l'argent dans des disques durs plus grands, plus performants, plutôt que dans un cache SSD. Si j'étais photographe, cependant, ou si j'avais beaucoup plus d'utilisateurs et, dans le meilleur des cas, un réseau local plus rapide, les choses seraient différentes. Dans le réseau d'entreprise, où chaque seconde d'attente coûte de l'argent, le cache SSD ne peut manquer à l'appel. Si j'avais ma propre entreprise.

J'espère vraiment que cet article vous donnera une idée des capacités et des applications d'un cache SSD. Si vous avez déjà utilisé un cache SSD, il serait bon de lire les commentaires sur l'augmentation de vitesse que vous obtenez grâce à lui. Si vous avez fait d'autres expériences avec le cache, par exemple si vous avez déjà dû échanger un SSD parce qu'il approchait de sa fin de vie, dites-le nous aussi !

Cet article plaît à 100 personne(s)

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