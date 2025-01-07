# Principles Of Web Accessibility

_Un ensemble de principes directeurs de haut niveau pour approcher l’accessibilité web._

* [L’ennemi c’est la perfection](#l-ennemi-c-est-la-perfection)
* [Par défaut, ou la mort](#par-defaut-ou-la-mort)
* [La Parité par-dessus tout](#la-parite-par-dessus-tout)
* [Concevez pour l’implémentation](#concevez-pour-l-implementation)
* [D’abord, la structure](#d-abord-la-structure)
* [Utilisez vos mots](#utilisez-vos-mots)
* [Les outils ne sont pas des identités](#les-outils-ne-sont-pas-des-identites)
* [Moins, c’est moins](#moins-c-est-moins)
* [Fais-toi payer](#fais-toi-payer)
* [La pèche, pas le poisson](#la-peche-pas-le-poisson)
* [Zéro point pour la performativité](#zero-point-pour-la-performativite)
* [Aidez à l’échec du mal](#aide-a-l-echec-du-mal)

## L’ennemi c’est la perfection

Rien n’est –ni ne peut être– accessible à 100 %. Quiconque revendique une offre complètement accessible est un menteur, ou ne comprend pas l’accessibilité, ou les deux. Généralement c’est les deux. C’est ok de livrer un travail inaccessible, à condition qu’il soit _davantage_ accessible qu’avant. Faites ce que vous pouvez au sein des contraintes données. Si les contraintes ne sont pas raisonnables, commencez par les questionner. Vous pouvez ne pas vous sentir la meilleure personne disponible pour travailler sur l’accessibilité. Mais vous _êtes disponible_. Ne laissez pas le travail à des super-héro·ïnes de l’accessibilité qui sont absentes (et n’existent pas).

## Par défaut, ou la mort

Fondamentalement, l’accessibilité ne marche pas comme un <i lang="en">plugin</i>, un <i lang="en">add-on</i> ou un état à activer. Si une interface offre l’option d’_activer_ l’accessibilité, elle est inaccessible. Un bouton à faible contraste qui déclenche un contraste élevé ? <i lang="en">Game over</i>. De manière catégorique : une surcouche d’accessibilité ne marche pas et ne peut pas marcher. Ajouter _des trucs d’accessibilité_ par dessus _des trucs inaccessibles_ ne répond pas aux besoins qui doivent être satisfaits. Les fonctionnalités spécifiques offertes par ces intrus tiers sont immatérielles. Résistez à tout prix à l’idéologie de l’accessibilité _post-hoc_. Un Produit Minimum Viable (MVP) pas accessible n’atteint même pas la viabilité miniumum.

## La Parité par-dessus tout

Le but n’est pas de créer une meilleure expérience, ou même une bonne expérience. C’est de s’assurer que différentes personnes auront des expériences _comparables_. Une interface ne doit pas être problématique pour certaines mais pas pour les autres, même si certaines interfaces sont complexes et certains contenus ésotériques. Vous n’avez pas à choisir qui s’intéresse à ça –ou qui peut le gérer. Si une image montre une blague, le texte alternatif ne doit pas gâcher la blague ni expliquer ce qui est drôle. Il doit _raconter la même blague par des moyens alternatifs_. La blague pourrait être choquante pour certain·es, ou inexplicable pour d’autres. Ce sont des manquements en matière d’inclusion, pas d’accessibilité.

## Concevez pour l’implémentation

On dit que la forme doit suivre la fonction. Mais beaucoup d’organisations conçoivent le design d’abord et développent ensuite. La phase de conception du design consiste purement en idéations graphiques et laisse trop de questions d’implémentation sans réponse. De ce fait, les devs se retrouvent encouragé·es à prioriser l’approximation visuelle plutôt que l’accessibilité. Les interfaces de glisser-déposer doivent être opérables avec un clavier. Ce qui veut dire que des boutons doivent être inclus. Ces boutons doivent apparaître dans le “_design_”. Dans la pratique de l’accessibilité, vous vous devez de contribuer au plus tôt dans un projet, dès l’étape de la conception. Parce que la forme doit suivre la fonction et la fonction doit être accessible.

## D’abord, la structure

Une interface mal structurée pourra techniquement être conforme aux <abbr>WCAG</abbr>  (Recommandations d'accessibilité des contenus Web). Une interface bien structurée et intuitive pourra comporter des erreurs de conformité multiples et distinctes. Mais il y a des chances que cette dernière soit l’interface accessible au plus grand nombre. Les outils d’accessibilité automatique ne sont vraiment bons qu’à repérer des erreurs isolées. Bien qu’ils puissent être utiles pour les diagnostics, vous devriez adopter une approche holistique. Qu’est-ce qui va troubler ou submerger les gens ? Où est-ce qu’ils vont se faire piéger ? Ne perdez pas de temps à cocher individuellement des critères de conformité lorsque la structure sous-jacente a besoin d’être repensée.

## Utilisez vos mots

Renseigner des libellés de texte représente une proportion considérable de l’accessibilité web. Les boutons, liens ou champs doivent tous avoir des libellés. De même, les en-têtes et la titraille des pages sont des types importants de libellés. Les messages de statut sont importants pour renseigner l’état de la page. Ajouter un libellé peut faire disparaître une alerte dans un test automatique, mais c’est le _texte_ de ce libellé qui va faire la différence. Une bonne rédaction ne peut pas être automatisée. L’intelligence artificielle ne peut pas anticiper votre intention. Développez vos compétences de rédaction, ou incluez des rédacteur·ices dans vos processus.

## Les outils ne sont pas des identités

Le handicap n’est pas plus uniforme que son absence. Différents utilisateurs de lecteurs d’écrans utilisent des lecteurs d’écrans différents de différentes manières pour différentes raisons dans des circonstances différentes pour satisfaire des besoins ou des préférences différentes. Et ça, c’est si elles utilisent un logiciel de lecteur d’écran. Il n’y a pas de persona qui puisse modéliser de manière adéquate un utilisateur de lecteur d’écran ou son comportement. Aucun utilisateur de lecteur d’écran ne parle au nom de tous les utilisateurs de lecteurs d’écran. Donc ne concevez pas pour “les utilisateurs de lecteurs d’écrans” (ou tout autre groupe homogène fictif). Concevez pour supporter les capacités des logiciels de lecteurs d’écrans. Les personnes ne peuvent –et ne doivent– pas être quantifiées, mais les entrées et sorties peuvent l’être et le sont.

## Moins, c’est moins

Le mantra <i lang="en">less is more</i>, _moins c’est plus_, est faux. Moins, c’est juste moins, et c’est une bonne chose. Il y a trop de décisions techniques d’interfaces qui sont prises parce que d’autres l’ont fait, ou juste pour prouver que c’est possible. Stop. Plus on ajoute, plus le résultat est complexe, plus le risque est grand que ça échoue. Et pas juste en produisant des erreurs ou des pannes isolées ; mais surtout en résistant à la compréhension. Dans la majorité des cas, la plupart des composants devrait être juste du contenu. Le contenu ne devrait que rarement être caché derrière un bouton. Transformer des titres, des paragraphes ou des listes en une interface à onglets accessible n’est pas une amélioration. C’est une dégradation, juste pour se vanter.

## Fais-toi payer

Ne permettez pas qu’on vous exploite pour votre enthousiasme pour l’accessibilité. Comme tout travail, plus il y a de gens qui le font gratuitement, moins il a de valeur. Le travail d’accessibilité n’est pas un extra, un hobby, ou une faveur. C’est une partie fondamentale d’un design d’interface de qualité. Si on vous paye pour travailler et que vous travaillez sur l’accessibilité, elle doit être dans la définition de votre rôle. Le travail d’accessibilité doit être reconnu et récompensé comme n’importe quel autre boulot. Là où _“l’accessibilité c’est le travail de tout le monde”_, c’est souvent celui de personne. Attention à ce genre de rhétorique.

## La pèche, pas le poisson

La conception de produits et interfaces accessibles commence par concevoir les organisations et communautés qui les feront. Tu peux faire du travail accessible aujourd’hui mais qui est-ce qui le fera demain ? Qui ou quoi pourrait le _défaire_ demain ? Concevoir accessible peut vouloir dire bâtir une équipe d’intégration composée de devs qui maitrisent l’intégration. Ça peut vouloir dire décommissionner un CMS qui interdit la production de contenus accessibles. Ça peut vouloir dire enseigner à une équipe éditoriale comment structurer leurs contenus. Si vous réparez l’inaccessibilité par vous-même, votre impact va vite s’estomper.

## Zéro point pour la performativité

Les entreprises ont tendance à préférer _avoir l’air_ d’améliorer l’accessibilité, plutôt que de réellement le faire. Elles recrutent des pros de l’accessibilité mais ne leur donnent pas les ressources nécessaires. Elles commissionnent des entretiens avec des personnes handicapées mais refusent d’interpréter les résultats. Elles payent pour des audits mais n’implémentent pas les recommandations. Elles vous disent que le contraste des couleurs doit être traité mais ne bougent pas sur le sujet sacré des couleurs de leur marque. Si vous voulez faire une réelle différence, exigez la pratique au lieu de la performativité.

## Aidez à l’échec du mal

Tout ce qui est inaccessible n’a pas à être accessible. Certaines choses ne devraient pas exister du tout. Si un produit ou une application est intrinsèquement abusive ou addictive, si elle produit de la désinformation ou de la haine, voire si simplement elle rajoute au malheur du monde, c’est mieux de la laisser être la cible d’un procès. Ne l’aidez pas à y échapper. Les propriétaires de tels produits ne méritent _aucun_ client ou utilisateur, et encore moins des personnes handicapées ou autrement marginalisées (qui pourraient être affectées de manière disproportionnée de par leurs pratiques). C’est votre jugement moral qui décide de la ligne entre l’acceptable et l’abject. Mais le fait de tracer une ligne quelque part contribue à la cohérence de votre offre en tant que praticien.
