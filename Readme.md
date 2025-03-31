Projet d'analyse de données de trajectoires dans Dota2

Réalisé par Etienne BOSSU, Alexandre FAUPOINT, Thomas DOGUET, Romain MOALIC


Modules utilisés : numpy, matplotlib, pandas, prefixSpan.


Différents types de fichiers executables dans src/ :
    fichiers main*.py : permettent de faire tourner l'algo sur toute les données
    fichiers display*.py : permettent de montrer les résultats de l'Algorithme
    fichiers compare*.py : nous on permit de comparer les algos selon le choix de paramêtres


Architecture du dossier data:
    raw/
        les csv donnés dans le sujet, contient les données xi, vec_xi, yi, vec_yi pour chaque Joueur i dans une partie ainsi que les ticks
    processed/
        les objets trajectoires extraits des csv avec leurs coordonnées normalisées au format JSON
    results/
        les résultats de nos algo (MDL, KMeans, PrefixSpan)


Architecture du dossier src:
    |algorithms/
        les classes de nos algorithmes
    |model/
        structure de données (trajectoire, points)
    |results/
        data_manager.py : Une classe qui nous permet de gérer les JSON, les CSV, etc
    |fichiers pythons executables
    
