---
layout: post
title: Les partis politiques québécois sont-ils cohérents?
excerpt: "La suite de notre analyse automatisée des stratégies de communication des partis politiques québécois."
modified: 05/05/2023, 18:55
tags: [analyse et fouille de textes, sciences humaines numériques, QDA Miner]
comments: true
category: blog
---

L’application de méthodes de fouille de textes (_text mining_ ou _text analytics_) gagne en importance auprès des partis politiques canadiens. Cette tendance met en évidence la pertinence, pour les chercheurs en science politique, de considérer ces procédés en contexte de recherche. Aussi avons-nous, Yutaka Suzuki et moi, soumis à divers algorithmes d'intelligence artificielle les plateformes électorales des cinq principaux partis politiques québécois. Ce billet de blogue fait le compte-rendu d'une partie de notre travail. Pour voir le reste de notre analyse, cliquez [ici](https://juste-un-roy.github.io/blog/Iramuteq-poltext1/).

### Mesurer la cohérence des partis politiques avec la méthode de la classification automatique ###

Une approche classique en fouille de textes se nomme la classification automatique. C'est cette approche qui nous a permis de prédire, avec une précision de 99%, quels partis politiques ont écrit les textes que nous lui avons soumis. Si d’aussi hauts taux de précision ont de quoi surprendre, ils indiquent que les cinq principales formations politiques québécoises sont, somme toute, cohérentes avec leurs idéologies respectives et assez distinctes les unes des autres. Ce qui ne les empêche pas d’avoir quelques atomes crochus.

En effet, les erreurs commises par un algorithme de classfication automatique peuvent nous éclairer sur les similarités entre certains partis politiques. Prenant exemple du [travail de Dominic Forest](http://dominicforest.me/fed2015/2015/10/15/des-machines-et-des-mots-les-partis-sont-ils-coherents/), nous avons donc observé la matrice de confusion extraite de nos expérimentations.

<iframe src='https://flo.uri.sh/visualisation/14270493/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:500px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/14270493/?utm_source=embed&utm_campaign=visualisation/14270493' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>

### La CAQ et le PLQ sont les partis politiques les plus souvent confondus ###

Les partis les plus fréquemment confondus sont la CAQ le PLQ. 24 communiqués de la CAQ ont été associés aux libéraux, contre 7 documents caquistes attribués au PLQ. Ces deux formations ont en commun de courtiser un électorat de centre-droit, et de mener [une chaude lutte pour se mériter le titre de « parti de l’économie »](https://lactualite.com/politique/quel-est-le-parti-de-leconomie/). Ce sont aussi deux partis ayant, au cours de la période couverte par notre corpus, formé un gouvernement, puis demandé aux Québécois et aux Québécoises de les réélire pour un deuxième mandat.

<iframe src='https://flo.uri.sh/visualisation/14272062/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:400px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/14272062/?utm_source=embed&utm_campaign=visualisation/14272062' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>


### Éric Duhaime courtise le vote caquiste ###

Le deuxième couple de partis les plus souvent confondus entre eux est composé de la CAQ et du PCQ. 8 communiqués du PCQ ont été attribués aux Conservateurs, contre 1 document caquiste associé aux PCQ. Cette dynamique traduit donc moins un « pas de deux » qu’une volonté du chef conservateur de courtiser les appuis caquistes. Rappelons qu'[Éric Duhaime a déjà persuadé une ancienne député de la CAQ de rejoindre ses rangs](https://www.tvanouvelles.ca/2021/06/18/claire-samson-rejoint-le-pcq-deric-duhaime) et déclaré qu’[il espérait rallier d’autres caquistes à sa cause](https://www.lapresse.ca/elections-quebecoises/2022-10-04/duhaime-reve-de-trouver-une-autre-claire-samson-a-la-caq.php). Enfin, la confusion entre ces partis politiques a pu être accentuée par la surreprésentation du mot « Legault » dans les communiqués du PCQ, qui a ancré son identité dans son opposition au premier ministre.

### François Legault ne se gène pas pour emprunter des idées à ses adversaires ###

En conclusion, soulignons que 34 textes émis par la CAQ ont été classé incorrectement. Ce parti a au moins un communiqué qui a été attribué à chaque parti de l'opposition. Doit-on y voir la stratégie de communication d’un parti attrape-tout, déterminé à rejoindre le plus grand nombre d’électeurs et électrices possible? Nos résultats brossent en effet le portrait d’une formation largement cohérente avec son idéologie, mais disposée à empiéter sur les terrains de ses adversaires de temps à autres.

<iframe src='https://flo.uri.sh/visualisation/14271873/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:300px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/14271873/?utm_source=embed&utm_campaign=visualisation/14271873' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>

### Corpus ###

Le corpus utilisé pour cette expérimentation est un ensemble de 4213 communiqués officiels récoltés sur les sites web des différentes formations politiques.

### Méthodologie ###

La classification naïve bayésienne est une approche courante en fouille de textes, relevant d'un apprentissage-machine supervisé. Elle repose sur le modèle probabiliste de Bayes et implique une forte indépendance statistique des caractéristiques d’un document. En d’autres termes, elle traite chacun des attributs d’un texte comme influant sur sa probabilité d’appartenir à l’une ou l’autre formation politique, sans égard pour la corrélation entre ces attributs. Son déploiement, comme celui des autres procédés relevant de l’apprentissage supervisé, nécessite un corpus d’apprentissage d’autant plus grand que sa taille doit être proportionnelle au nombre de catégories - ou de partis - mobilisées.
