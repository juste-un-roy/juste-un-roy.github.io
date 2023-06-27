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

__Mesurer la cohérence des partis politiques avec la méthode de la classification automatique__

Une approche classique en fouille de textes se nomme la classification automatique. Elle nous a permis d'amener une intelligence artificielle à prédire, avec une précision de 99%, quels partis politiques ont écrit les textes dans notre corpus.

D’aussi hauts taux de précision ont de quoi surprendre, considérant la petite taille de notre corpus et le grand nombre de catégories mobilisées (en règle générale, plus on emploie de catégories, plus la précision de l'intelligence articielle baisse). Aussi croyons-nous pouvoir en déduire que les cinq principales formations politiques québécoises sont, somme toute, cohérentes avec leurs idéologies respectives et assez distinctes les unes des autres. Ce qui ne les empêche pas d’avoir quelques atomes crochus.

En effet, après s’être félicité de la qualité des résultats obtenus, nous avons souhaité étudier les erreurs commises par l'intelligence artificielle, avec l’espoir qu’elles relèveraient des similarités entre certains partis politiques. Prenant exemple du [travail de Dominic Forest](http://dominicforest.me/fed2015/2015/10/15/des-machines-et-des-mots-les-partis-sont-ils-coherents/), nous avons donc observé les matrices de confusion extraites de nos expérimentations.

<iframe src='https://flo.uri.sh/visualisation/14270493/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:500px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/14270493/?utm_source=embed&utm_campaign=visualisation/14270493' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>

__La C.A.Q. et le P.L.Q. : en lutte pour être le « parti de l'économie »__

La première source d’erreurs digne d’intérêt est une confusion proéminente entre les textes émis par la C.A.Q. et les communiqués du P.L.Q. Ces deux formations ont effectivement plusieurs points en commun, notamment d’occuper un espace au centre droit du spectre politique et de mener une chaude lutte pour se voir attribuer l’épithète de « parti de l’économie ». Ce sont aussi deux partis ayant, au cours de la période couverte par notre corpus, formé le gouvernement, puis demandé aux québécois de les réélire pour un deuxième mandat. Enfin, à la fois la C.A.Q. et le P.L.Q. courtisent l’électorat qui se place au centre de l’axe gauche-droite. Quoiqu’en disent leurs représentants, ces organisations semblent donc entretenir une relation de similarité assez forte pour confondre une intelligence artificielle.

<iframe src='https://flo.uri.sh/visualisation/14272062/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/14272062/?utm_source=embed&utm_campaign=visualisation/14272062' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>


__Éric Duhaime en quête de « caquistes déçus »__

Une autre source d’erreurs notable implique encore une confusion entre la C.A.Q. et un autre parti politique, cette fois le P.C.Q. Ceci étant dit, elle semble moins traduire un « pas de deux » qu’une velléité du chef conservateur de courtiser les appuis caquistes. Hypothèse que corroborent les faits, Duhaime ayant déjà persuadé une ancienne député de la C.A.Q. de rejoindre ses rangs et déclaré qu’il espérait convertir d’autres « caquistes déçus ». D’autant que le P.C.Q. a été le plus compétitif dans des circonscriptions acquises à la C.A.Q. depuis 2012, comme Beauce-Nord. Par ailleurs, la confusion entre ces partis politiques aurait pu être accentuée par la sur-représentation du mot « Legault » dans les communiqués du P.C.Q., caractéristique d’une formation qui a ancré son identité dans son opposition au premier ministre.

__François Legault ne se gène pas pour emprunter à ses adversaires__

Finalement, il convient de souligner que la classification naïve bayésienne a prédit incorrectement le parti politique de 34 textes émis par la C.A.Q., avec un nombre d’erreurs à peu près égal pour Q.S. et le P.Q. Doit-on y voir la stratégie de communication d’un parti centriste, déterminé à rejoindre le plus grand nombre d’électeurs possible ? On pourrait, en tout cas, émettre l’hypothèse que les confusions avec le P.Q. découlent de l’emploi fréquent, autant par les itérations de ce parti postérieures à 2007 que par L’équipe François Legault, d’un vocabulaire associé au nationalisme identitaire. Quant aux confusions avec Q.S., elles pourraient résulter des mesures adoptées par le gouvernement caquiste en environnement, un thème cher à la formation de gauche. Tous ces éléments brossent le portrait d’une formation largement cohérente avec son idéologie, mais disposée à empiéter sur les terrains de ses adversaires.

<iframe src='https://flo.uri.sh/visualisation/14271873/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/14271873/?utm_source=embed&utm_campaign=visualisation/14271873' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>

__Corpus__

Le corpus utilisé pour cette expérimentation est le même que celui décrit [dans mon précédent billet de blogue](https://juste-un-roy.github.io/blog/Iramuteq-poltext1/).

__Méthodologie__

La classification naïve bayésienne est une approche courante en fouille de textes, relevant d'un apprentissage-machine supervisé. Elle repose sur le modèle probabiliste de Bayes et implique une forte indépendance statistique des caractéristiques d’un document. En d’autres termes, elle traite chacun des attributs d’un texte comme influant sur sa probabilité d’appartenir à l’une ou l’autre formation politique, sans égard pour la corrélation entre ces attributs. Son déploiement, comme celui des autres procédés relevant de l’apprentissage supervisé, nécessite un corpus d’apprentissage d’autant plus grand que sa taille doit être proportionnelle au nombre de catégories - ou de partis - mobilisées.
