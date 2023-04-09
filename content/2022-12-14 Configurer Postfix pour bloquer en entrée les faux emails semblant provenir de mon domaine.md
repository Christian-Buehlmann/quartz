
---
title: "2022-12-14 Configurer Postfix pour bloquer en entrée les faux emails semblant provenir de mon domaine"
---

## Configurer Postfix pour bloquer en entrée les faux emails semblant provenir de mon domaine

Quand j'ai reçu un énième email semblant émaner de ma propre adresse emails et me réclamant du pognon pour ne pas dévoiler que je me pignole sur du porn, je me suis dit que, quand même, il doit exister un moyen de bloquer ça sans recourir à un antispam. Je m'en suis jamais préoccupé jusque-là car j'en reçois très peu, mais j'ai désormais du temps pour creuser la question, donc autant en profiter. \o/
 
Contexte : je n'ai pas d'antispam sur mon serveur emails personnel, pas besoin (il suffit de filer sa véritable adresse à des gens de confiance et de filer une adresse générique ‒ un alias ‒ ou la véritable en y ajoutant un [délimiteur / tag](https://en.wikipedia.org/wiki/Email_address#Sub-addressing) aux autres, et surtout aux sociétés commerciales, aux windowsiens et aux listes de discussion archivées sur le web). J'ai un seul serveur emails pour mon domaine personnel. J’utilise le MTA Postfix.
http://shaarli.guiguishow.info/?axiAUQ

[[- InternetScrap]]

[[- Cybersécurité]]