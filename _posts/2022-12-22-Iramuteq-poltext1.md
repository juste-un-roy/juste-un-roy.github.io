---
layout: post
title: Quels sont les mots caractéristiques des partis politiques québécois?
excerpt: "De simples opérations en fouille de textes peuvent nous informer sur les stratégies de communication des partis politiques québécois."
modified: 22/01/2023, 11:33
tags: [analyse et fouille de textes, sciences humaines numériques, Iramuteq]
comments: true
category: blog
---
L’application de méthodes de fouille de textes (_text mining_ ou _text analytics_) gagne en importance auprès des partis politiques canadiens. Cette tendance met en évidence la pertinence, pour les chercheurs et chercheuses en science politique, de considérer ces procédés en contexte de recherche. Aussi avons-nous, Yutaka Suzuki et moi, soumis à divers algorithmes d'intelligence artificielle les plateformes électorales des principaux partis politiques québécois. Ce billet de blogue fait le compte-rendu d'une partie de notre travail.

__Analyser le discours des partis politiques avec la méthode du calcul des spécificités__

Inspirés par les travaux de Dominic Forest et de Damon Mayaffre, nous avons recouru au calcul des spécificité pour relever les mots caractéristiques de 5 partis : la Coalition avenir Québec (CAQ) ; le Parti libéral du Québec (PLQ) ; Québec solidaire (QS) ; le Parti québécois (PQ) ; le Parti conservateur du Québec (PCQ).

<iframe src='https://flo.uri.sh/visualisation/14225684/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/14225684/?utm_source=embed&utm_campaign=visualisation/14225684' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>

__Coalition Avenir Québec__

Les mots « enfant », « scolaire » et « décrochage » sont surreprésentés dans les documents programmatiques de cette formation. Cette spécificité concorde avec [les nombreuses allocutions lors desquelles François Legault a affirmé qu'une de ses priorités était l’éducation](https://ici.radio-canada.ca/nouvelle/1138225/assemblee-nationale-session-priorites-immigration) ; elle découle peut-être aussi du fait que [la CAQ a souvent courtisé le vote des familles](https://www.lesoleil.com/2017/11/26/la-caq-promet-detre-le-gouvernement-des-familles-0b8bd6104e005d4b74e68dabc76c2779/). Notons que ces termes sont aussi surreprésentés au PCQ, tout comme l'est « contribuable ». Les deux formations, campées à droite de l'axxe politique, semblent donc se disputer un même électorat.

__Parti Libéral du Québec__

Les documents programmatiques de ce parti affichent une sur-représentation de termes génériques. Les mots à saveur procédurale, comme « conseil », « membre », « exécutif » ou « comité » , y abondent. Cette absence de contenu idéologique, au sein même des documents pourtant censés traduire l’orientation politique du P.L.Q., pourrait refléter un mal qui gangrène le parti depuis quelques années, à savoir que [la formation peine à redéfinir son identité](https://www.lapresse.ca/debats/editoriaux/2022-09-28/parti-liberal-du-quebec/a-la-recherche-d-une-identite-perdue.php) à une époque marquée par la disparition progressive du clivage souveraineté-fédéralisme. La perte en vitesse de ce débat, qui profitait encore à Charest en 2003, semble avoir privé le Parti libéral d'un projet central, inscrit dans la longue durée. Rappelons toutefois que la plateforme électorale complète du parti pour 2022 n'était pas accessible au moment de constituer notre corpus.

__Québec Solidaire__

Les mots « droit », « femme », « peuple » et « autocthone » sont sur-représentés au sein des documents programmatiques de ce parti marqué à gauche de l'échiquier politique, mais sous-représentés chez les autres formations. Le thème de la démocratie et de la citoyenneté, exprimé par les mots « participatif », « collectivité » et « citoyen », distingue également Q.S. Certains parallèles entre les formes caractéristiques de QS celles et des autres partis s’avèrent dignes de mention. D’abord, soulignons qu'à la fois QS et le PQ se démarquent par leur surutilisation des mots « communautaires », « travailleur », « public » et « social ». Puis, que le PCQ comme QS emploient plus souvent que les autres formations les termes « alternative », caractéristique d’une posture contestataire, et « public », lequel fait écho à un sujet sur lequel les deux partis s’opposent : celui du financement des services publics.

__Parti Québécois__

La surreprésentation des mots « fier », « protéger », « français », « indépendance » et « nation » évoque le caractère nationaliste de cette formation traditionnellement attachée à la protection de la langue française et à la séparation du Québec du reste du Canada. À cet égard, soulignons deux choses. D’abord, que le terme « indépendance » est sous-représenté chez QS, [une formation pourtant indépendantiste](https://ici.radio-canada.ca/nouvelle/1392944/souverainete-environnement-canada-congres-quebec-solidaire-independance). Puis, que « français » est aussi surutilisé par la CAQ, [qui a déposé une refonte de la Loi 101 plus tôt en 2022](https://ici.radio-canada.ca/nouvelle/1885719/loi-96-vote-pq-plq-opposition). Pour revenir au PQ, la surrutilisation de certains mots associés à la transition énergétique - « énergétique », « émission », « réduction » - traduisent une fibre écologiste.

__Parti Conservateur du Québec - Équipe Éric Duhaime__

Les documents programmatiques du PCQ que nous avons pu trouver traduisent des enjeux de la dernière campagne électorale. La surutilisation des mots « logement », « locataires » et «loyer » indique que la formation semble avoir fait de la question du logement une priorité, [bien qu'elle nie l'existence d'une crise du logement](https://www.conservateur.quebec/famille_et_logement). Sur ce point, notons que les mots « privé » et « marché », aussi surreprésentés dans les documents programmatiques des Conservateurs, sont généralement employés lorsque le parti propose supprimer des initiatives gouvernementales en matière de logement. On pourait s'étonner que la formation d'Éric Duhaime surrutilise le mot « subventionner » ; mais celui-ci est utilisé négativement par le parti, tout comme « tramway », qui fait référence à [un projet de transport en commun auquel s’opposait son chef](https://www.journaldequebec.com/2022/09/27/eric-duhaime-mettrait-rapidement-la-hache-dans-le-tramway). Enfin, la surreprésentation des mots « sanitaire » et « urgence » évoque l'importance du thème de la gestion de la crise pandémique pour ce parti.

__Corpus__

Notre corpus rassemble les documents programmatiques émis par les cinq principaux partis politiques québécois entre 2007 et 2022. Il couvre les plateformes électorales des formations et leurs programmes ; il exclut les messages publiés par les partis sur les réseaux sociaux et les documents à saveur administrative comme les règlements.

Malheureusement, les plateformes électorales pour l’année 2022 du PLQ et du PQ n’étaient pas accessibles en ligne au moment où nous avons constitué notre corpus. Nous avons compensé ce manque en récoltant plusieurs documents officiels portant sur des enjeux spécifiques, comme le développement économique des régions et l’indépendance du Québec. Par ailleurs, aucun document émis par le PCQ avant 2020 n’était acessible en ligne au moment de créer notre corpus. Le profil de cette formation représente donc uniquement les orientations que lui a données son nouveau chef, Éric Duhaime.

__Méthodologie__

Le [modèle du calcul des spécificités de Lafon](https://www.persee.fr/doc/mots_0243-6450_1980_num_1_1_1008) propose de comparer la fréquence d’un mot dans un corpus en entier avec sa fréquence dans un échantillon donné. Cette approche permet de distinguer les mots dont la présence dans un texte pourrait relever du hasard (0) de ceux qui s'éloignent du modèle soit positivement (+1) ou négativement (-1). Les mots qui s'éloignent positivement du modèle sont surreprésentés dans l'échantillon, tandis que les mots qui s'en éloignent négativement sont sous-représentés.
