---
title: "<% tp.file.title %>"
---

[[- InternetScrap]]
[[ReadItLater]] [[Article]]

# [Écarter les développeurs open source menace le fonctionnement des systèmes informatiques](https://www.silicon.fr/avis-expert/ecarter-les-developpeurs-open-source-menace-le-fonctionnement-des-systemes-informatiques)

  ![Programmation IDE Orion Eclipse web open source © Vicente Barcelo Varona - Shutterstock](private/ReadItLater%20Inbox/assets/Programmation%20IDE%20Orion%20Eclipse%20web%20open%20source%20©%20Vicente%20Barcelo%20Varona%20-%20Shutterstock.jpg)

Qu’il s’agisse de créer une nomenclature de logiciels pour les applications utilisées par une organisation ou de soutenir les projets et les développeurs de logiciels open source, les entreprises doivent redoubler d’efforts pour contribuer à réduire leurs risques.

Les logiciels informatiques sont au cœur de toutes les entreprises et [jouent un rôle crucial](https://www.silicon.fr/open-source-moteur-economie-europeenne-415795.html) à tous les niveaux opérationnels. Presque toutes feront appel à des logiciels open source, sciemment ou non, puisque même les logiciels propriétaires dépendent de bibliothèques open source.

En France, le marché du logiciel open source poursuit sa progression. Il représente aujourd’hui 11% du marché du numérique et 16% des services, [selon une étude](https://cnll.fr/news/etude-2022-le-march%C3%A9-de-lopen-source-en-france-et-europe/) présentée conjointement par le CNLL, Numeum et Systematic Paris-Région.

Les entreprises exigent de plus en plus d’informations concernant les systèmes essentiels à leur fonctionnement, ce qui les poussent à s’intéresser de près à la chaîne d’approvisionnement en matière de logiciels. Elles créent une nomenclature logicielle ([Software Bill of Materials – SBOM](https://www.cisa.gov/sbom)) pour chacune de leurs applications grâce à laquelle elles peuvent identifier avec certitude les logiciels et les modèles utilisés, ainsi que les systèmes concernés. La maîtrise de ces informations représente un atout majeur en cas de faille de sécurité.

## Une grande dépendance à l’égard de la communauté bénévole

Fin 2021, la faille de sécurité Log4Shell [a été identifiée](https://www.silicon.fr/log4shell-ecosysteme-cyber-reponse-422310.html) au sein d’un système de logging Java largement utilisé : Log4j. Cette bibliothèque open source étant largement utilisée, la vulnérabilité a fait l’objet d’une importante médiatisation et des corrections étaient attendues.

Toutefois, les personnes chargées de la maintenance du projet étaient des bénévoles avec des emplois réguliers et qui n’étaient donc pas en mesure d’apporter des réponses immédiates aux problèmes de sécurité, quand bien même un grand nombre de systèmes étaient touchés. Selon les estimations, cette vulnérabilité [a affecté](https://www.itespresso.fr/log4shell-ce-quil-faut-savoir-sur-la-faille-java-qui-seme-la-panique-261204.html) 93% des infrastructures cloud des entreprises.

L’open source suscitait auparavant une certaine méfiance, mais la réalité est que si ce composant avait été un logiciel propriétaire, la faille n’aurait peut-être jamais été connue du public et les organisations auraient pu être victimes d’attaques. Le fait est que la nature open source de la bibliothèque a permis qu’elle soit examinée, que les anomalies soient détectées et que des conseils puissent être donnés par divers contributeurs.

Ainsi, les bénévoles chargés de la maintenance du projet ne se sont pas inquiétés d’éventuels risques de sécurité. La grande question reste de savoir comment s’est-on retrouvé dans une situation où de grandes entreprises dépendent d’un logiciel dont la maintenance n’est pas encadrée par des dispositions contractuelles.

Ne pas prendre en compte les mécanismes de dépendance des systèmes constitue un risque, quelle que soit la licence du logiciel. Mais lorsque celui-ci est open source et très largement utilisé, cela devient encore plus problématique. Dans le cas présent, le problème existait dans le code depuis plusieurs années, mais n’avait jamais été détecté. Bien qu’il soit largement utilisé, cet outil ne disposait pas en réalité d’une assistance à sa mesure.

Cette histoire se répète régulièrement dans de nombreuses entreprises qui dépendent de logiciels sensibles, sans prendre de mesures pour soutenir les personnes chargées de leur maintenance ou des projets en question. Disposer d’un SBOM pour le système utilisé par une entreprise implique que cette dernière dispose des informations nécessaires. Pour les organisations fournissant des logiciels à des tiers, la mise à disposition du SBOM en parallèle du code tend à se normaliser.

## Identifier les points de dépendance pour mieux évaluer les risques

Connaître l’état des dépendances simplifie l’évaluation du risque associé à chacune d’entre elles. Les projets open source sont les plus évidents à analyser : a-t-on répondu aux problèmes et y a-t-il eu des versions récentes ? La possibilité de consulter les personnes chargées de la maintenance et des activités de chaque projet permet d’avoir un aperçu de sa bonne santé. Pour réduire les risques, les entreprises peuvent intervenir soutenant les projets dont elles sont dépendantes.

Certains le sont directement via le programme de parrainage de GitHub, d’autres sont plutôt ouverts aux offres d’hébergement ou d’audit de sécurité, mais tous les projets open source apprécient les contributions tierces. Si l’entreprise crée elle-même cette bibliothèque, les développeurs de l’entreprise devront résoudre le moindre dysfonctionnement par leurs propres moyens.

Il faut envisager l’open source comme un système de propriété partagée. L’objectif n’est pas de construire le même système de façon répétitive, mais d’y contribuer, ce qui implique un effort moindre et une meilleure efficacité. L’une des mesures les plus pertinentes que les entreprises peuvent adopter est de mobiliser leurs ressources techniques et de contribuer à la correction de certains dysfonctionnements ou à la création de nouvelles fonctionnalités pour des projets qui sont au cœur de leur activité.

Maintenir ses propres experts impliqués dans un projet présente de nombreux avantages. Ils en acquièrent une meilleure connaissance et peuvent surveiller les nouvelles fonctionnalités ainsi que la disponibilité de nouvelles versions. L’entreprise dispose en outre d’un aperçu de la santé et de l’état du projet en question et participe à son bon fonctionnement, réduisant ainsi le risque d’un incident lié à la dépendance.

Un certain nombre d’organisations disposent d’un OSPO (open source program office), dont les collaborateurs se consacrent à la contribution, voire à la maintenance, des programmes utilisés. Ces services contribuent souvent [à la visibilité globale de l’entreprise](https://www.silicon.fr/open-source-europe-constat-cru-fondation-linux-447366.html) dans l’écosystème open source et permettent aux autres collaborateurs d’y participer plus facilement.

Une autre approche consiste à soutenir les organisations existantes qui appuient les projets open source. Par exemple, l[‘OpenSSF](https://openssf.org/) (Open Source Security Foundation) vise à améliorer la sécurité des projets open source et est financée par les organisations qui dépendent de ces projets. Elle publie également des ressources documentaires utiles afin que les entreprises puissent s’informer sur les risques associés aux logiciels qu’elles utilisent.

On peut également citer une autre organisation similaire baptisée [Tidelif](https://tidelift.com/)t qui s’associe aux mainteneurs de projets open source afin de garantir le respect de certaines exigences de base, et est également financée par les organisations.

## Assurer un avenir plus sûr pour les logiciels

Il existe aujourd’hui une dépendance des entreprises vis-à-vis de l’informatique, et notamment des logiciels open source qui sont largement utilisés et généralement plus sûrs que les solutions propriétaires.

Il s’agit d’une démarche ingénieuse, mais qui le sera d’autant plus si l’on dispose d’une vision claire de la chaîne d’approvisionnement des logiciels et de ses dépendances. Lorsqu’un problème survient, le fait d’être dépendant de projets robustes et de disposer des données détaillées bénéficie à chaque organisation. Si elles agissent toutes ainsi, le risque d’événements malheureux tels que la faille de Log4Shell aurait été considérablement réduit.