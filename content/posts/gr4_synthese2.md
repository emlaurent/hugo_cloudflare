Le séchoir solaire réduit l'humidité contenue dans un produit pour
empêcher le développement de micro-organismes. Ainsi la déshydratation
d'un aliment lui octroie une durée de conservation bien plus longue.
L'utilisation de cette technique peut rendre accessible les aliments en
dehors de leur saison naturelle de production et réduire le gaspillage
alimentaire. De plus, en tant que low-tech, le séchoir peut être
construit facilement, avec des matériaux accessibles. Enfin,
l\'utilisation d'énergie solaire présente un réel atout pour la
transition énergétique.

Choix du cas d\'usage
---------------------

Pour pouvoir modéliser le séchoir solaire et l\'optimiser, un cas
d\'usage doit être choisi. Nous avons considéré une implantation au
Sénégal au regard de plusieurs critères. En effet, le potentiel solaire
du pays, la place importante qu\'y occupe l\'agriculture et les pertes
post-récoltes conséquentes sont favorables à l\'implémentation du
séchoir solaire. Par manque d\'infrastructures et d\'accès à
l\'électricité, il n\'existe que peu voire pas de systèmes concurrents
dans les régions isolées du Sénégal. Les pertes importantes à la récolte
s\'observent notablement pour les mangues et les oignons, deux aliments
parfaitement adaptés au séchage solaire.

> Pour une argumentation d\'avantage détaillée, voir livrable 2 :
> https://pad.lamyne.org/GENEPI\_2022\_L2\_final\_\_GRP3.

Le modèle de déshydrateur considéré est le séchoir solaire indirect
forcé. Ce choix correspond à un compromis entre efficacité de séchage et
qualité des fruits, mais le séchoir indirect forcé n\'est pas forcément
le plus adapté pour tous les cas d\'usage. La taille du séchoir
envisagée correspond à une utilisation individuelle par des petits
producteurs ou bien des coopératives, le nombre de séchoirs pouvant
augmenter.

Le fonctionnement d\'un tel séchoir dans ce cas d\'usage, est détaillée
dans la partie suivante et dans le livrable 1
(https://pad.lamyne.org/GENEPI\_2022\_L1\_GRP3).

Fonctionnement du séchoir et modélisation
-----------------------------------------

Le séchoir solaire indirect est divisé en deux parties: le collecteur et
la chambre de séchage.
![](https://hot-objects.liiib.re/pad-lamyne-org/uploads/1c4568f1-4c6d-443e-9ad8-4a53fbb5f500.png)
https://www.lesagronautes.org/index.php/2019/11/22/secher-ses-aliments-avec-des-materiaux-de-base-et-lenergie-du-soleil/

*Fonctionnement du collecteur* Le collecteur permet d\'augmenter la
température de l\'air ambiant afin qu\'il atteigne une température
optimale pour le séchage de fruit. Il est constitué d\'une grande caisse
disposée en pente. L\'entrée de l\'air se fait au niveau du sol et la
sortie de l\'air chaud coïncide avec l\'entrée de la chambre de séchage
(située plus en hauteur). La partie supérieure de la caisse est en verre
afin de pouvoir laisser passer les rayons du soleil. Les parois internes
doivent être peintes en noir afin d\'absorber un maximum d\'énergie
solaire. L\'étude des paramètres impactant le séchage des fruits nous a
permis de conclure que les deux paramètres primaires sont la température
de l\'air et son taux d\'humidité dans le caisson de séchage. C\'est
pour cela que des petits ventilateurs (type ventilateurs de PC) sont
ajoutés à l\'entrée ou à la sortie du collecteur. Ils permettent de
contrôler le débit d\'air et donc la température en sortie de
collecteur. Des petits panneaux solaires permettent de faire fonctionner
ces ventilateurs. L\'augmentation de la température de l\'air permet
aussi d\'abaisser son taux d\'humidité bien en dessous de 70% afin que
le séchage des fruits soit possible. (cf annexe)

------------------------------------------------------------------------

*Modélisation du collecteur*:

L\'entrée du modèle est le flux solaire incident transmis à travers la
vitre. Cette puissance thermique est soit transmise (ce que l\'on
souhaite) à l\'air qui circule dans le collecteur , soit perdue vers des
zones froides du collecteur.

Les pertes thermiques dans le collecteur ont lieu par convection
(transfert de chaleur par mouvement des masses d\'air au sein du
collecteur), par conduction (transfert de la chaleur de proche en proche
dans la vitre du collecteur) et par rayonnement (transfert de la chaleur
qui atteint la vitre extérieure du collecteur par émission de photons
vers l\'environnement qui est plus froid).

On utilise l\'analogie thermique-électrique (cf. Annexe) pour décrire
les transferts thermiques dans le collecteur. En posant les équations
associées au schéma électrique (cf. Livrable 3
https://shorturl.at/ghkKT) où ces calculs sont détaillés(IV.4) et où le
schéma électrique est représenté (IV.3)), **on isole la température de
l\'air en sortie du collecteur. Ce paramètre est déterminant dans le
calcul de l\'évolution du taux d\'humidité dans la chambre de séchage**
dont le fonctionnement sera détaillé plus loin.

A noter que l\'on obtient finalement une température de sortie de
collecteur pour chaque heure de la journée où le séchoir est en
fonctionnement. Pour déterminer le taux d\'humidité des fruits et le
rendement du séchoir on a consiéré comme température de sortie la
moyenne des températures de sortie pour chaque heure.

Après avoir étudié l\'influence des paramètres intervenant dans le
calcul des résistances et donc de la température de sortie de l\'air on
arrive aux conclusions suivantes:

-   La présence d\'un double vitrage permet de diminuer
    significativement les pertes par rapport à un simple vitrage.
-   Le débit d\'air imposé par le ventilateur et la surface du
    collecteur sont des paramètres déterminants dans la température de
    sortie.

------------------------------------------------------------------------

*Fonctionnement de la chambre de séchage* Une fois que l\'air est chaud
et sec, il arrive dans la chambre de séchage. La chambre est un caisson
rectangulaire isolant dans lequel plusieurs grilles sont disposées les
unes sur les autres comme dans un four. Les fruits préalablement coupés
sont étalés sur ces grilles. Il est essentiel de noter que la découpe
des fruits est un paramètre important pour l\'efficacité du séchage
surtout vers la fin du processus : plus les morceaux sont petits plus la
surface d\'échange avec l\'air est grande et moins l\'eau doit se
déplacer par capillarité : le séchage est d\'autant plus rapide. L\'air
chaud va s\'élever naturellement à travers les grilles qui peuvent être
de n\'importe quel matériau mais doivent avoir des trous assez grands et
non obstrués par les fruits pour faciliter la circulation. Au contact de
l\'air chaud et sec, l\'eau contenue par les fruits va s\'évaporer.
Grâce au ventilateur le débit d\'air est maintenu afin que l\'air qui
devient humide au fur et à mesure de sa montée dans la chambre soit
évacué par une cheminé se trouvant sur le haut du caisson.

*Modélisation de la chambre de séchage* Le séchage des fruits fait
intervenir de nombreux phénomènes complexes, qui ne sont pas modélisés
dans le détail. Le modèle réutilise plutôt des formules tirées d\'études
spécialisées (voir Annexe) afin d\'évaluer l\'évolution de l\'humidité
des fruits selon la température. On obtient ainsi le temps de séchage
estimé, et indirectement le rendement de la chambre dans les conditions
définies par l\'utilisateur.

L\'utilisation conjointe des modèles de collecteur et de chambre de
séchage permet ainsi d\'évaluer l\'impact des dimensions du premier sur
les performances de séchage dans le second. On peut alors identifier les
paramètres de premier ordre, évaluer comment évolue la capacité selon
chaque paramètre, et après confrontation avec des résultats
expérimentaux s\'en servir comme outil de dimensionnement.

Retour sur la modélisation
--------------------------

L\'étude chiffrée du séchoir solaire modélisé a été réalisée dans le but
d\'évaluer son efficacité et sa performance pour l\'optimiser. Les
conditions météorologiques moyennes retenues sont celles d\'un mois de
juillet au Sénégal, période qui correspond à la récolte des mangues.
Plusieurs hypothèses simplificatrices ont été prises en compte lors de
l\'établissement de ce modèle. L\'exploitation d\'équations
mathématiques nous a permis de modéliser l\'évolution de la teneur en
eau présente dans les mangues au cours du séchage. Un fruit est
considéré comme séché lorsque sa teneur en eau est inférieure à 20%.

A partir de la modélisation, il a également été possible de déduire un
rendement global du déshydrateur solaire qui n\'est autre que le produit
du rendement du collecteur et du rendement du séchage. Ce rendement
global s\'exprime comme le rapport entre l\'énergie utilisée pour
chauffer et évaporer l\'eau présente dans les fruits et l\'énergie
solaire disponible sur une surface identique à celle de l\'absorbeur.
Pour les conditions météorologiques choisies, le rendement global obtenu
avec le modèle est de 11,6 %. Cette valeur est légèrement supérieure à
celles données dans la littérature pour des expériences aux conditions
similaires. Ceci peut s\'expliquer par les simplifications faites
notamment dans le modèle du collecteur qui sous-estime légèrement les
pertes thermiques.

En faisant varier les paramètres du modèle il a été possible de
déterminer ceux qui influencent le plus les performances du système. Il
est alors nécessaire de trouver un équilibre entre masse de fruits à
sécher, la surface du collecteur et la vitesse de l\'air. La variation
de ces paramètres impacte grandement la température et l\'humidité de
l\'air qui eux déterminent l\'efficacité du séchage.

Ainsi, pour 8 kg de mangue, un capteur de 1,9 m² et un air à une vitesse
de 0,8 m/s, on trouve un temps de séchage de 54,5 h ce qui concorde avec
les données de la littérature scientifique.

Validité du cas d\'usage
------------------------

Au cours de notre étude, nous avons eu l\'occasion de rencontrer un
diplômé de l\'Insa Lyon du département GEn, qui a travaillé en Afrique
Subsaharienne. Les informations qu\'il a pu nous apporter ont permis de
confirmer la viabilité de notre cas d\'usage : les populations
Subsaharienne sont habituées à manger des fruits séchés, les matériaux
nécessaires tels que les panneaux solaires sont accessibles sur les
marché locaux et des projets de ce genre voient déjà le jour
actuellement. Seul point négatif pour notre cas d\'usage : la saison des
mangues est pluvieuse, empêchant donc une utilisation optimale des
séchoirs solaires. Il serait pertinent de s\'intéresser à d\'autres
fruits ou légumes qui sont produits à différentes saisons. Enfin, la
modélisation de notre séchoir solaire nous a permis d\'obtenir des
résultats de rendement permettant un séchage optimal des aliments dans
les conditions climatiques du Sénégal.
