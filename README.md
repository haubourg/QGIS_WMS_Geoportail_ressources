QGIS_WMS_Geoportail_ressources
==============================

Série de ressources pour faciliter l'utilisations des flux WMS WMTS Geoportail dans QGIS. 

Outils pour simplifier l'intégration de raccourcis vers les couches WMS WMTS servies par IGN

Auteur Régis Haubourg 
regis.haubourg@eau-adour-garonne.fr

version 1.1
date 3 octobre 2013

Contenu :
projets QGIS:
 - Donnees_IGN_Geoportail.qgs : projet pour QGIS 1.8 (WMS vecteurs uniquement, projection 2154)
 - Donnees_IGN_Geoportail_qgsv2.qgs : projet pour QGIS 2.0 , projection 3857, échelles de tuiles intégréespour flux WMTS geoportail (incompatible v2)

fichiers d'export des échelles de tuiles (déjà intégrées dans le projet QGIS v2, fonctionnalité inexistante dans QGIS 1.8)
 - geoportail_scales.xml : export des échelles rélles (avec virgules) définies par le Geoportail en projection 3857
 - geoportail_scales_arrond.xml: export des échelles arrondies (bug QGIS si décimales) à importer dans les propriétés du projet en projection 3857.


Mode d'emploi:
- télécharger les fichiers sur Github (à droite "Download zip") 
- Créer un compte sur professionnel.ign.fr puis commandez les services API Geoportail pour SIG (gratuit pour des missions de service public) http://professionnels.ign.fr/services. Vous obtiendrez une série de clés et identifiants pour les services Geoportail et INSPIRE
- ouvrir avec un bloc note le projet qgs compatible avec votre version de QGIS. Les fichiers d'échelles sont déja intégrés dans le projet  Donnees_IGN_Geoportail_qgsv2.qgs. 
- rechercher -remplacer les 6 valeurs suivantes avec les valeurs récupérées sur votre compte IGN.

MonUserNameINSPIRE 
MonUserPasswordINSPIRE
MonUserNameGEOPORTAIL
MonUSerPasswordGEOPORTAIL
MaCleINSPIRE
MaCleGEOPORTAIL


- ouvrir le projet QGIS 
Pensez à régler vos paramètres de proxy si besoin. Il peut subsister des erreurs de saisie de login / mdp dans le qgs, corriger à la main.. n'hésitez pas à me le signaler, ou à proposer directement des corrections via github

--- pour créer des raccourcis vers ces données, installer le plugin "layers menu from project", puis Extension/Menu Layers from project / configurer les projets.  http://plugins.qgis.org/plugins/menu_from_project/ 

Ajouter le projet QGIS de votre version dans la liste. et c'est tout!

Les évolutions coté services semblent signalées sur le blog de l'API ign : http://api.ign.fr/blog Il manque juste un flux rss



