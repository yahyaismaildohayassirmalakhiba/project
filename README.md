#projet c:

1. chargerVoitures(const char* nomFichier)

    Objectif : Charger les informations des voitures à partir d'un fichier CSV et les stocker dans un tableau de structures Voiture.
    Entrée : Le nom du fichier CSV (chaîne de caractères) qui contient les données des voitures.
    Sortie : Aucune (fonction void). Les données lues sont directement stockées dans le tableau global voitures.
    Détails : La fonction ouvre le fichier en mode lecture, lit chaque ligne et extrait les informations sur les voitures à l'aide de la fonction fscanf. Ces informations sont ensuite stockées dans le tableau voitures. Le nombre de voitures lues est suivi par la variable nombreVoitures. Si l'ouverture du fichier échoue, un message d'erreur est affiché.

2. sauvegarderVoitures(const char* nomFichier)

    Objectif : Sauvegarder les informations des voitures présentes dans le tableau voitures dans un fichier CSV.
    Entrée : Le nom du fichier CSV où les données seront sauvegardées.
    Sortie : Aucune (fonction void). Les informations des voitures sont écrites dans le fichier spécifié.
    Détails : La fonction ouvre le fichier en mode écriture ("w"), puis utilise fprintf pour écrire les données de chaque voiture dans le fichier CSV sous le format :

    id, marque, modèle, typeCarburant, places, transmission, prixParJour, disponible

    Si l'ouverture du fichier échoue, un message d'erreur est affiché.

3. afficherVoitures()

    Objectif : Afficher la liste des voitures avec leurs détails dans la console.
    Entrée : Aucune.
    Sortie : Aucune (fonction void). La fonction affiche simplement les informations des voitures sur la console.
    Détails : Cette fonction affiche un en-tête contenant les titres des colonnes, puis parcourt le tableau voitures et imprime les informations de chaque voiture, telles que l'ID, la marque, le modèle, le type de carburant, le nombre de places, la transmission, le prix par jour, et la disponibilité. Si une voiture est disponible, elle est indiquée comme "Disponible", sinon "Non disponible".

4. ajouterVoiture()

    Objectif : Ajouter une nouvelle voiture dans le tableau voitures.
    Entrée : Aucune (l'utilisateur saisit les informations de la voiture via la console).
    Sortie : Aucune (fonction void). La nouvelle voiture est ajoutée au tableau voitures.
    Détails : La fonction vérifie d'abord si le nombre maximum de voitures a été atteint. Si ce n'est pas le cas, elle demande à l'utilisateur de saisir les informations de la voiture (marque, modèle, type de carburant, nombre de places, transmission, prix par jour). Ensuite, la voiture est ajoutée au tableau, et le compteur nombreVoitures est incrémenté. Par défaut, la voiture est marquée comme "disponible" (disponible = 1).
