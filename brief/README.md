# Kékés Voyages (UML + MERISE)


## Table des matiéres

- [Régles de gestion](#régles-de-gestion)


## Régles de gestion

**Client** : 

    - Doit s'indetifié pour réservé.
    - Peut choisir un aéroport de départ et d'arrivé.
    - Peut choisir l'heure de départ.
    - Peu annuler le vol reservé.
    - Peut demandé une réservation de vol.
    - Peut choisir lors de la réservation la place dans l'avion.
    - Peut resérver pour plusieurs passagers.

**Vol (Trajet)** : 
    - A une heure de départ et d'arrivé.
    - A un aéroport de départ et d'arrivé.
    - Peut avoir des éscales (changement d'avion et d'aéroport).
    - Peut avoir une ville de départ et d'arrivé.
    - A un identifiant de vol.

**Compagnie aérienne** : 
    - Peut ajouter, annuler des vols.
    - Confirmer une demande de réservation.
    - Refuser une demande de réservation.
    - Peu changer les horaires d'un vol.
    - Peu chamger les escales d'un vol.
    - Verfie l'identification lors de la demade de réservation.
    - Peu annulé la reservation d'un client ou d'un passagé.

**Avion** : 
    - Peu changer pendant une escale.
    - A un numéro d'appareil.
    - Nombre de passagers limité.

**Passagers** : 
    - A une place reservé par le client ou lui même.
    - Doit posseder un élement d'identification.
    - Est dans une certaine tranche d'âge.

## Usecase Diagrams

