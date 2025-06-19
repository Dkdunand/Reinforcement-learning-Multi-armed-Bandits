# Restless Bandits & Robust Exploration: A Theoretical and Experimental Study
# Objectif
Ce projet explore la robustesse des algorithmes de bandits manchots classiques dans un cadre non stationnaire, inspiré des environnements financiers réels. Nous étudions les bandits "restless", un cadre où les distributions de récompense évoluent avec le temps, contrairement au modèle i.i.d. traditionnel.

L’objectif est d’évaluer comment les politiques d’exploration-exploitation — cruciales pour la prise de décision séquentielle — se comportent lorsqu’on les applique hors de leur cadre théorique optimal.

 # Contexte
🔬 Bandits manchots à bras finis, où les récompenses sont dépendantes temporellement.

 Basé sur le cadre présenté par Grunewalder & Khaleghi (2019).

Ce type de désalignement est analogue à de nombreux problèmes rencontrés en finance algorithmique, où les rendements sont souvent autocorrélés et non stationnaires.

# Méthodologie
Nous appliquons l’algorithme UCB1 (Auer et al., 2002), conçu pour des environnements i.i.d., à des données générées par des processus dépendants.

L’objectif est d’observer l’impact de cette dépendance sur les performances et de déterminer si des ajustements sont nécessaires.

# Expérimentations :

Comparaison des performances UCB1 sous différentes intensités de dépendance temporelle.

Simulations multiples avec échantillonnage contrôlé pour quantifier la dégradation des performances.

 Extensions prévues
Si le temps le permet, nous étendrons cette étude à :

 Bandits linéaires, avec l’algorithme LinUCB (Lattimore & Szepesvári, 2020)

 Comparaison avec LinMix-UCB (Khaleghi, 2025), conçu pour les environnements non-i.i.d.

 # Pourquoi ce projet est pertinent pour un hedge fund ?
 Exploration-exploitation en environnement incertain = cœur de l’allocation dynamique d’actifs.

 Modélisation de la non-stationnarité des marchés : ce projet examine des situations analogues aux changements de régime, effets mémoire, autocorrélation.

 Capacité à évaluer la robustesse algorithmique, une compétence clé en stratégie systématique.

 Combinaison de recherche appliquée et d’implémentation expérimentale, avec une attention portée à la réalité opérationnelle.

 # Références clés
Auer et al. (2002) – Finite-time Analysis of the Multiarmed Bandit Problem

Grunewalder & Khaleghi (2019) – Restless Bandits with Temporal Dependencies

Lattimore & Szepesvári (2020) – Bandit Algorithms (Ch. 19)

Khaleghi (2025) – LinMix-UCB: Bandit Learning with Structured Temporal Dependence




