---
layout: post
title: Quels sont les mots caractéristiques des partis politiques québécois?
excerpt: "De simples opérations en fouille de textes peuvent nous informer sur les stratégies de communication des partis politiques québécois."
modified: 22/01/2023, 11:33
tags: [analyse et fouille de textes, sciences humaines numériques, Iramuteq]
comments: true
category: blog
---
L’application de méthodes de fouille de textes (_text mining_ ou _text analytics_) gagne en importance auprès des partis politiques canadiens. Cette tendance met en évidence la pertinence, pour les chercheurs en science politique, de considérer ces procédés en contexte de recherche. Aussi avons-nous, Yutaka Suzuki et moi, soumis à divers algorithmes d'intelligence artificielle les plateformes électorales des cinq principaux partis politiques québécois. Ce billet de blogue fait le compte-rendu d'une partie de notre travail.

__Analyser le discours des partis politiques avec la méthode du calcul des spécificités__

Inspirés par les travaux de Dominic Forest et de Damon Mayaffre, nous avons d'abord recouru à la méthode du calcul des spécificités. Celle-ci nous a permis de relever les mots caractéristiques des formations à l'étude : la Coalition avenir Québec - L’équipe François Legault (C.A.Q.-E.F.L.) ; le Parti libéral du Québec/Quebec Liberal Party (P.L.Q./Q.L.P.) ; Québec solidaire (Q.S.) ; le Parti québécois (P.Q.) ; le Parti conservateur du Québec - Équipe Éric Duhaime (P.C.Q-E.E.D.).

<iframe src='https://flo.uri.sh/visualisation/14225684/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/14225684/?utm_source=embed&utm_campaign=visualisation/14225684' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>

__Coalition Avenir Québec - L'équipe François Legault__

![CAQ](https://user-images.githubusercontent.com/110431473/236683431-4d0d1b4c-8243-4369-a879-dc5f75ebea46.PNG)

Les mots « enfant », « scolaire » et « décrochage » se retrouvent parmi les plus caractéristiques des plateformes électorales et documents programmatiques de cette formation. Cette spécificité concorde avec les nombreuses allocutions lors desquelles François Legault a affirmé que sa priorité était l’éducation  ; elle découle peut-être aussi du fait que la C.A.Q. a souvent courtisé un électorat composé de jeunes familles. Par ailleurs, notons que ces termes sont sous-représentés chez Q.S. et sur-représentés au P.C.Q. Le terme « contribuable », afférent au thème de l’économie, évoque la position sur l’échiquier politique de cette formation, campée à droite et soucieuse du portefeuille des québécois pris individuellement. Fait intéressant, ce même mot est sur-représenté dans les textes du P.C.Q., un autre parti de droite, mais sous-représenté au P.L.Q., lequel s’est pourtant longtemps défini comme le « parti de l’économie ».

__Parti Libéral du Québec - Quebec Liberal Party__

![PLQ](https://user-images.githubusercontent.com/110431473/236683439-fc8a02d1-8fe7-4c0b-8410-9b4cb85bc789.PNG)

Les documents programmatiques de ce parti affichent une sur-représentation de termes trop larges pour évoquer un positionnement idéologique. Les mots à saveur procédurale, comme « conseil », « membre », « exécutif » ou « comité » , y abondent. Cette absence de contenu idéologique, au sein même des documents pourtant censés traduire l’orientation politique du P.L.Q., pourrait refléter un mal qui gangrène le parti depuis quelques années, à savoir que la formation de Couillard et Anglade peine à redéfinir son identité, à une époque marquée par la disparition progressive du clivage souveraineté-fédéralisme. La perte en vitesse de ce débat, qui profitait encore à Charest en 2003, semble avoir privé le Parti libéral d'un projet central, inscrit dans la longue durée.

__Québec Solidaire__

![QS](https://user-images.githubusercontent.com/110431473/236683451-6a2ac665-e7e1-4364-ae0c-d4409bb84150.PNG)

Les mots « droit », « femme », « peuple » et « autocthone » sont sur-représentés au sein des documents programmatiques de ce parti, qui se réclame du féminisme et de la défense des groupes minoritaires, mais sous-représentés chez les autres formations. Le thème de la démocratie et de la citoyenneté, exprimé par les mots « participatif » (comprendre « démocratie participative »), « collectivité » et « citoyen », distingue également Q.S. Certains parallèles entre les formes caractéristiques de Q.S. et des autres partis s’avèrent dignes de mention. D’abord, soulignons que le P.Q. utilise aussi les mots « communautaires », « travailleur », « public » et « social », qui traduisent la sensibilité de gauche des deux partis, plus aiguë à Q.S. Plus évocateur encore, le P.C.Q. partage avec Q.S. les termes « alternative », caractéristique d’une posture clivante ou contestataire, et « public », lequel fait écho à un sujet sur lequel les deux partis s’opposent : celui du financement des services publics.

__Parti Québécois__

![PQ](https://user-images.githubusercontent.com/110431473/236683465-3846130e-9efa-44b2-b830-066f705ec5ec.PNG)

La sur-représentation des mots « fier », « protéger », « français », « indépendance » et « nation » dénote le caractère nationaliste de cette formation traditionnellement attachée à la protection de la langue française et à la séparation du Québec du reste du Canada. À cet égard, soulignons deux choses. D’abord, que le terme « indépendance » est sous-représenté chez Q.S., une formation pourtant indépendantiste, comme elle l’est chez la C.A.Q., le P.C.Q. et le P.L.Q. Puis, que « français » est aussi sur-utilisé par la C.A.Q., un parti nationaliste, mais sous-représenté chez le P.L.Q., le P.C.Q. et Q.S., lesquels prônent plutôt des formes de cosmopolitisme ou d’internationalisme. Pour revenir au P.Q., quelques mots associés à la transition verte - « énergétique », « émission », « réduction » - traduisent sa fibre écologiste. De même, quelques mots à connotation positive - « gagnant », « aspirer », « réussir » - brossent le portrait d’un parti optimiste dans ses revendications.

__Parti Conservateur du Québec - Équipe Éric Duhaime__

![PCQ](https://user-images.githubusercontent.com/110431473/236683477-4cad1b87-c61f-46d6-ab22-7c70ae1e4b84.PNG)

Les documents programmatiques du P.C.Q., en faible nombre, traduisent surtout les enjeux de la dernière campagne électorale. Outre le nom et l’acronyme de la formation, on y trouve maints termes relatifs à la question du logement.  Comme Q.S., qui sur-utilise aussi le mot « logement », cette formation semble avoir fait de la crise du logement une priorité. Ses solutions diffèrent toutefois de celles préconisées par la formation de gauche, et reflètent plutôt une vision libertarienne de l’économie. Aussi retrouve-t-on « marché » (entendre « libre-marché ») parmi les formes caractéristiques du P.C.Q. Ensuite, figurent les thèmes de la santé et de la gestion de la crise pandémique, lesquels transparaissent à travers divers mots, tels « sanitaire » et « urgence ». Sur ces questions encore, s’exprime la philosophie économique du parti : le mot « privé », lui aussi très fréquent, est employé lorsque le P.C.Q. propose de privatiser le secteur de la santé au Québec. À cet égard, on pourrait s’étonner du score du mot « subventionner » ; mais compte tenu de ce qui a été dit, on peut déduire que celui-ci est utilisé négativement par le parti, tout comme « tramway », qui fait référence à un projet de transport en commun auquel s’opposait la formation en 2022.

__Corpus__

Notre corpus rassemble les documents d'importance émis par les cinq principaux partis politiques québécois entre le 23 août 2018 et le 3 octobre 2022, ainsi qu’une poignée de textes programmatiques remontant jusqu’à l’année 2007. Il couvre les plateformes électorales des formations et leurs programmes ; il exclut les communications diffusées par des candidats individuels, les messages publiés par les partis sur les réseaux sociaux et les documents à saveur administrative comme les règlements.

Malheureusement, les plateformes électorales pour l’année 2022 du P.L.Q. et du P.Q. n’étaient plus accessibles en ligne au moment d’effectuer le moissonnage des données. Nous avons compensé ce manque en récoltant plusieurs documents officiels portant sur des enjeux spécifiques, comme le développement économique des régions et l’indépendance du Québec. Par ailleurs, aucun document émis par le P.C.Q. avant 2020 n’était disponible en ligne à cette date. Le profil de cette formation représente donc uniquement les orientations que lui a données son nouveau chef, Éric Duhaime.

__Méthodologie__

Le modèle du calcul des spécificités de Lafon propose de prendre comme point de référence, ou comme norme, la fréquence absolue d’une forme dans le corpus entier, puis de le mettre en relation avec sa fréquence absolue dans un échantillon aléatoire du même corpus. Cette approche permet de distinguer les occurrences dont la présence pourrait relever du hasard (formes de base), de celles qui s'éloignent du modèle (formes spécifiques), soit positivement (sur-représentées) ou négativement (sous-représentées).
