Guide d\'utilisation
--------------------

-   **Fonctionnement du modèle Excel**

*Collecteur*

L\'analogie thermique électrique fonctionne de la façon suivante:

-   Les températures sont les potentiels du circuit
-   Les différences de température sont les tensions du circuit
-   Le flux thermique est l\'intensité dans le circuit.

Le flux solaire incident transmis arrive sur le noeud central du circuit
qui correspond à la température moyenne de l\'air. Le flux se sépare
ensuite en deux branches: la première branche correspond au chauffage de
l\'air et la deuxième aux pertes vers l\'extérieur.

Le schéma électrique, le détail des calculs ainsi que l\'ensemble des
hypothèses simplificatrices sont détaillées dans le livrable 3
(https://shorturl.at/ghkKT).

*Chambre de séchage*

A défaut de s\'appuyer sur un modèle descriptif des phénomènes physiques
de séchage, la simulation s\'appuie sur des lois établies
expérimentalement (loi de Page). Celles-ci sont propres au fruit étudié
et aux conditions de température et d\'humidité. Elles permettent de
calculer au cours du temps l\'évolution du ratio d\'humidité selon la
température. La température moyenne en sortie de collecteur, déjà
obtenue par modélisation, sert alors d\'entrée. Le ratio d\'humidité
permet ensuite d\'accéder à d\'autres indicateurs utiles comme le taux
d\'humidité et donc le temps de séchage. Le modèle nécessite pour ces
calculs l\'humidité spécifique, qui s\'obtient à partir de l\'humidité
relative (voir diagramme d\'air humide). De même, il calcule l\'humidité
spécifique en sortie de collecteur, qui doit être encore convertie en
humidité relative avant de tirer toute information sur la capacité de
l\'air à absorber l\'humidité.

-   **Utilisation du modèle Excel**

Le modèle proposé permet d\'évaluer les performances d\'un séchoir
solaire selon certains paramètres géométriques et thermiques. Par
extension, c\'est un outil pour évaluer l\'impact de ces paramètres, et
pour s\'assurer que les conditions décrites permettent le séchage. Les
paramètres ajustables sont ainsi entrés dans les cases *jaunes* du
tableur. A l\'inverse, les cases *rouges* ne doivent surtout pas être
éditées car critiques pour le bon fonctionnement des calculs. Pour
simuler le séchage dans de nouvelles conditions, après avoir rentré les
paramètres souhaités, il est nécessaire de mettre à jour la feuille
Excel : pour cela, se placer dans la case E27 et incrémenter toute la
colonne en double-cliquant dans le coin inférieur droit. Les
informations alors obtenues telles que les rendements du système, ou le
temps de séchage, sont rassemblées dans le tableau \"RESULTATS\".
Attention toutefois avant de tirer des conclusions : ce modèle possède
une **plage de validité**, tant en humidité relative qu\'en température,
en dehors de laquelle les résultats ne sont plus exploitables. Il
convient en effet de s\'assurer à chaque simulation que ces conditions
sont respectées : si les cases de température moyenne (L18) et
d\'humidité spécifique (J27 et en dessous) se colorent en rouge, la
valeur sort du cadre de l\'étude.

-   **Utilisation du diagramme d\'air humide et analyse de l\'évolution
    de l\'humidité relative dans l\'air du séchoir**

Le diagramme d\'air humide (voir figure 1) permet de calculer comment va
varier l\'évolution de l\'humidité de l\'air entre l\'entrée du
collecteur et la sortie de celui-ci à partir de trois données: la
température de l\'air extérieur et son humidité ainsi que la température
de sortie du collecteur. (La température de l\'air en sortie du
collecteur peut être estimée avec le débit d\'air entrant, sa
température, le flux solaire et le rendement du collecteur). Il est
important de noter que le diagramme en figure 1 est valable pour des
pressions extérieures proches de la pression atmosphérique standard
(101325 Pa). L\'abcisse du diagramme est la température en degré. Sur
l\'axe des ordonnées il y a à la fois l\'humidité spécifique de l\'air
et la pression de vapeur d\'eau. L\'humidité spécifique correspond à la
masse d\'eau contenue par kg d\'air sec tandis que la pression de vapeur
d\'eau correspond à la pression liée à la vapeur d\'eau dans l\'air. Les
courbes rouges indiquent quant à elles l\'humidité relative de l\'air,
c\'est à dire le rapport de la pression de vapeur d\'eau sur la pression
de vapeur saturante de l\'eau dans l\'air à cette même température.

Pour déterminer l\'humidité relative en sortie du collecteur et la
quantité d\'eau qu\'il peut encore absorber par masse d\'air sec, il
faut commencer par se placer en entrée du collecteur sur le diagramme,
c\'est à dire à l\'intersection entre la courbe d\'humidité relative de
l\'air extérieur et la verticale partant de la température extérieure.
Ensuite, il faut se translater à l\'horizontale sur le graphique jusqu'à
atteindre l\'abscisse correspondant à la température de sortie du
collecteur. Il est alors possible de relever entre quelles courbes
d\'humidité relative (10%, 20%, 30%, etc.) ce nouveau point est situé.
C\'est ce qui permet d\'estimer quelle est la nouvelle humidité relative
de l\'air. Pour savoir quelle quantité d\'eau cet air peut encore
absorber, il faut relever l\'humidité spécifique (donc l\'ordonée du
point de sortie du collecteur), et relever l\'humidité spécifique
correspondant à 100% d\'humidité relative pour la même température. Cela
correspond à trouver l\'ordonnée du point à l\'intersection entre la
verticale partant de la température de sortie du collecteur et la courbe
d\'humidité relative indicée 100%. La différence entre l\'humidité
spécifique à 100% d\'humidité relative et celle en sortie du collecteur
permet de déterminer quelle masse d\'eau peut encore être absorbée par
l\'air.

![](https://hot-objects.liiib.re/pad-lamyne-org/uploads/28d0744d-e849-42ed-8780-ac4191fbfeb2.jpg)
Figure 1 : diagramme d\'air humide à pression atmosphérique

Liens utiles
------------

-   bibliographie Zotéro:
    https://www.zotero.org/groups/4800924/genepi\_2022\_23/collections/DZ3UNJU9
-   livrable 1: https://pad.lamyne.org/GENEPI\_2022\_L1\_GRP3
-   livrable 2: https://pad.lamyne.org/GENEPI\_2022\_L2\_final\_\_GRP3
-   livrable 3:
    https://docs.google.com/document/d/1PhF4NpRpoLh\_c5-LGhe\_gbHujmiOcEDVKyhNOnIlKPw/edit?usp=share\_link
