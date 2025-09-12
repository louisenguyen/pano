# Contexte


# Objectifs et principe


# Datasets

Panneaux : 

Routes : [troncon_de_route_44](https://data.geopf.fr/telechargement/download/BDTOPO/BDTOPO_3-5_TRANSPORT_GPKG_LAMB93_FXX_2025-06-15/BDTOPO_3-5_TRANSPORT_GPKG_LAMB93_FXX_2025-06-15.7z)


# Installation des composants

Installation postgresql (version) / postgis, python (version, venv ?)

# Intégration des datasets dans la base postgresql

Pre-requis : créer une base postgresql, importer la table troncon_de_route du gpkg dedans sous le nom de troncon_de_route_bd_topo

# Lancement des scripts

## Filtrage des données BDTopo

script(s) : [1_filtrage_troncon_pour_rattachement](1_filtrage_troncon_pour_rattachement.sql)
inputs : 
outputs : 


## Rattachement

### rattachement à partir de données contenant la position et l'orientation des panneaux

script(s) : [rattachement_pano_troncon_bdtopo_correction7_valide](rattachement_pano_troncon_bdtopo_correction7_valide.sql)
inputs : 
outputs : 

### rattachement à partir de données contenant la position et l'orientation des panneaux

script(s) : [2_script_rattachement_cd44_panneaux.sql](2_script_rattachement_cd44_panneaux.sql)
inputs : table 
outputs : 


## Préparation du graphe


### Segmentation

script(s) : 
inputs : 
outputs : 

### Optimisation

script(s) : 
inputs : 
outputs : 

## Calcul des vitesses