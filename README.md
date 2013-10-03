QGIS_WMS_Geoportail_ressources
==============================

Tools to facilitate IGN French Geoportail access with QGIS

Auteur Régis Haubourg 
regis.haubourg@eau-adour-garonne.fr

version 1
date 3 octobre 2012

Contenu :
Donnees_IGN_Geoportail.qgs : projet pour QGIS 1.8 (WMS vecteurs uniquement, projection 2154)
Donnees_IGN_Geoportail_qgsv2.qgs : projet pour QGIS 2.0 , projection 3857, échelles de tuiles pour flux WMTS geoportail (incompatible v2)
geoportail_scales.xml : export des échelles rélles (avec virgules) définies par le Geoportail en projection 3857
geoportail_scales_arrond.xml: export des échelles arrondies (bug QGIS si décimales) à importer dans les propriétés du projet.


Mode d'emploi:

- Obtenirles clés, login, et mots de passe IGN INSPIRE et GEOPORTAIL sur professionnel.ign.fr
- ouvrir avec un bloc note le projet compatible avec votre version de QGIS
- rechercher -remplacer les 6 valeurs suivantes avec les valeurs récupérées sur votre compte IGN

MonUserNameINSPIRE 
MonUserPasswordINSPIRE
MonUserNameGEOPORTAIL
MonUSerPasswordGEOPORTAIL
MaCleINSPIRE
MaCleGEOPORTAIL

- ouvrir le projet QGIS 
Pensez à régler vos paramètres de proxy si besoin. Il peut subsister des erreurs de saisie de login / mdp dans le qgs, corriger à la main.. 

--- pour créer des raccourcis vers ces données, installer le plugin "layers menu from project", puis Extension/Menu Layers from project / configurer les projets. 
Ajouter le projet QGIS de votre version dans la liste. et c'est tout!




