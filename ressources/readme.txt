
Auteur R�gis Haubourg 
regis.haubourg@eau-adour-garonne.fr

version 1
date 3 octobre 2012

Contenu :
Donnees_IGN_Geoportail.qgs : projet pour QGIS 1.8 (WMS vecteurs uniquement, projection 2154)
Donnees_IGN_Geoportail_qgsv2.qgs : projet pour QGIS 2.0 , projection 3857, �chelles de tuiles pour flux WMTS geoportail (incompatible v2)
geoportail_scales.xml : export des �chelles r�lles (avec virgules) d�finies par le Geoportail en projection 3857
geoportail_scales_arrond.xml: export des �chelles arrondies (bug QGIS si d�cimales) � importer dans les propri�t�s du projet.


Mode d'emploi:

- Obtenirles cl�s, login, et mots de passe IGN INSPIRE et GEOPORTAIL sur professionnel.ign.fr
- ouvrir avec un bloc note le projet compatible avec votre version de QGIS
- rechercher -remplacer les 6 valeurs suivantes avec les valeurs r�cup�r�es sur votre compte IGN

MonUserNameINSPIRE 
MonUserPasswordINSPIRE
MonUserNameGEOPORTAIL
MonUSerPasswordGEOPORTAIL
MaCleINSPIRE
MaCleGEOPORTAIL

- ouvrir le projet QGIS 
Pensez � r�gler vos param�tres de proxy si besoin. Il peut subsister des erreurs de saisie de login / mdp dans le qgs, corriger � la main.. 

--- pour cr�er des raccourcis vers ces donn�es, installer le plugin "layers menu from project", puis Extension/Menu Layers from project / configurer les projets. 
Ajouter le projet QGIS de votre version dans la liste. et c'est tout!




