```{=html}
<style>

h4
    {
      display: block;
    }
    h4
    {
      font-size : 60%;
      text-align : center;
      font-style: italic;
      color:darkblue;
    }
    div {
        text-align:justify;
    }
</style>
```
```{=html}
<style>
.alinea { 
  text-indent: 20px; 
}
</style>
```
### Présentation du système technique

```{=html}
<p class="alinea">
Le dessalinisateur choisi est un capteur solaire constitué d'un cadre en bois, d'une paroi vitrée exposée au soleil et d'un tissu à l'intérieur du panneau dans lequel circule de l'eau de mer à purifier. Les rayons du soleil traversent la vitre, chauffent le tissu qui monte en température et l'eau salée s'évapore. Cette vapeur d'eau s'élève pour venir se condenser sur la paroi de verre. Sous l'effet de la gravité, l'eau s'écoule le long de la paroi inclinée et est récupérée en bas du cadre. 
Ce système dispose des avantages suivants : 
```
-   simplicité de fabrication, des matériaux
-   adaptabilité et facilité d\'appropriation

```{=html}
<img style="display: block; margin: 0 auto;" src="https://hot-objects.liiib.re/pad-lamyne-org/uploads/3a5236f3-09b1-4d0c-93d8-1c16ec2d0158.png" width="95%">
<h4>Figure 1 : schéma de principe du dessalinisateur selon de système de C. Grandpierre</h4>
```
```{=html}
<p class="alinea">
Cependant, il faut garder à l'esprit que ce système ne permet pas de fournir de l'eau potable, mais seulement de l'eau douce.
```
### Choix d\'un cas d\'usage

```{=html}
<p class="alinea">
Lors de ce projet, une des question principale concernait le cas d'usage du dessalinisateur. Dans quel cas est-il intéressant de fabriquer et d'utiliser ce système? 
<p class="alinea">
Pour répondre à cela, nous nous sommes intéressés aux problèmatiques principales liées aux besoins en eau : l'accessibilité à l'eau et la consommation d'eau. Pour cela une notion clé a été introduite : le stress hydrique. Cela représente le rapport entre l'eau douce prélevée sur une année et la quantité totale de ressources en eau douce dans un territoire. 
<p class="alinea">
Cependant, ce paramètre ne suffit pas à lui seul car les pays plus développés ont recours aux dessalinisateurs industriels et à l'importation pour subvenir à leurs besoins. Après une étude complète de ces deux facteurs (disponible sur le livrable 2), et en considérant en priorité les populations ayant un accès direct à l'eau de mer, nous avons sélectionné le cas d'usage d'un village côtier nigérien. Un objectif serait de distribuer un dessalinisateur à chaque foyer d'un village. 
Avec ce modèle de développement, il semble judicieux de se placer en tant qu'ONG, qui produit et distribue directement au Nigéria.
```
### Synthèse de la modélisation

`<a href="https://cloud.lamyne.org/apps/files/?dir=/Communs%20Low-tech/GENEPI_2022_23/Equipe%20G5/Livrables&openfile=361524" >`{=html}Livrable
3`</a>`{=html}

```{=html}
<p class="alinea">
Après avoir émis des hypothèses simplificatrices, nous sommes parvenus à un modèle mathématique pour notre système, résumé par un schéma électrique équivalent (cf Figure 6 p.14, <a href="https://cloud.lamyne.org/apps/files/?dir=/Communs%20Low-tech/GENEPI_2022_23/Equipe%20G5/Livrables&openfile=361524" >Livrable 3 </a>). 
```
```{=html}
<p class="alinea">
Comme mentionné dans le <a href="https://cloud.lamyne.org/apps/files/?dir=/Communs%20Low-tech/GENEPI_2022_23/Equipe%20G5/Livrables&openfile=361524" >Livrable 3</a>, ce schéma des transferts de chaleurs de notre système a été établi par analogie électrique. Les résistances représentent les freins à la transmission de chaleur d’un noeud de température à un autre (couche d'air, paroi vitrée...). Sur le schéma, elles sont positionnées "en série" lorsque les transferts se font successivement et "en parallèle" lorsqu'ils se font à travers le même matériau/la même matière. 
```
En électricité, au niveau d'une résistance \$R\$ traversée par un
courant \$I\$, la tension \$U\$ s\'obtient grâce à la relation \$U =
R\\times I\$. De la même façon, en transfert de chaleur, au niveau d'une
résistance \$R\$ traversée par un flux \$\\Phi\$, le calcul de la
différence de température \$\\Delta T\$ s\'exprime par : \$\\Delta T =
R\\times \\Phi\$. Ainsi, pour les transferts conductifs, il suffit de
s'appuyer sur la Loi de Fourier \[hypertexte\] unidimentionelle à
travers un mur d\'épaisseur \$e\$ : on exprime la variation de
température en fonction du flux et on égale le coefficient devant le
flux obtenu à une résistance pour obtenir la formule de résistance
conductive présentée dans le
`<a href="https://cloud.lamyne.org/apps/files/?dir=/Communs%20Low-tech/GENEPI_2022_23/Equipe%20G5/Livrables&openfile=361524" >`{=html}Livrable
3`</a>`{=html} (cf partie 3.b.i). Pour les autres transferts de
chaleurs, l\'évaporation et la condensation, l\'inverse du coefficient
\$h\$ devant le flux pourrait s\'obtenir de la même manière, à partir
des expressions de flux associées. Cependant, celles-ci s\'avérant
complexes dans notre cas d\'étude, nous nous sommes contentés d\'estimer
ce coefficient \$h\$ en s\'appuyant sur des résultats connus, comme nous
le verrons par la suite.

Afin de bien comprendre ce schéma et les calculs qui s\'ensuivent, il
est nécessaire de rappeler les méthodes de résolution d'un circuit
électrique. Tout d\'abord, afin de simplifier le circuit, nous avons
besoin de réduire le nombre de résistances dans le circuit. Pour cela,
il suffit de sommer les résistances en série (séparées par un point dont
la température n\'est pas indispendable à la résolution du circuit) afin
d\'obtenir une résistance équivalente. C\'est par exemple ainsi que nous
avons déterminé \$R\_{fond}\$. Pour les résistances en parallèle,
l\'inverse de la résistance équivalente s\'obtient comme la somme de
l\'inverse de chaque résistance. Par exemple, cela nous a permis
d\'obtenir \$R\_{int}\$.

Une fois le circuit simplifié, la loi des noeuds s'applique au niveau
d'un noeud (croisement de plusieurs flux arrivants/sortants) : la somme
des flux arrivants est égale à la somme des flux partants de ce noeud.
Chaque noeud de notre schéma électrique nous donne ainsi une équation
que le système doit satisfaire. Afin d\'obtenir un système d\'équations
résoluble analytiquement (cf système d\'équation, partie 3.b.ii.,
`<a href="https://cloud.lamyne.org/apps/files/?dir=/Communs%20Low-tech/GENEPI_2022_23/Equipe%20G5/Livrables&openfile=361524" >`{=html}Livrable
3`</a>`{=html}), c\'est-à-dire avec autant de températures inconnues que
d\'équations fournies par les noeuds, le schéma électrique a été
amplement simplifié. Dans ce but, nous avons réalisé plusieurs
hypothèses répertoriées dans la partie 3.a. du
`<a href="https://cloud.lamyne.org/apps/files/?dir=/Communs%20Low-tech/GENEPI_2022_23/Equipe%20G5/Livrables&openfile=361524" >`{=html}Livrable
3`</a>`{=html}. Un glossaire est disponible dans les annexes afin de
définir le vocabulaire technique employé.

```{=html}
<p class="alinea">
Toutes les formules étudiées précédemment ont été reportées , il est à noter que les coefficients d’échanges thermiques eux-mêmes dépendent de paramètres physiques des composants du système et de ses environs. Alors, nous avons distingué quelques paramètres sur lesquels il faut porter notre attention :
```
-   **Flux solaire incident considéré** Selon le jour considéré, l'heure
    à laquelle le dessalinisateur est utilisé ou encore la météo du
    moment (couverture nuageuse), le flux solaire à considérer pour la
    modélisation du système varie. Il serait alors judicieux de faire
    varier la valeur du flux solaire, de façon à couvrir un maximum de
    cas de figure lors de l'étude du modèle proposé.

-   **Angle d'inclinaison du dessalinisateur** Le quantité de flux
    solaire incident sur la plaque de verre dépend de l'inclinaison de
    celle-ci. En effet, on peut définir un angle d'incidence des rayons
    solaires sur la plaque, dont la valeur intervienderait sur celle du
    flux solaire final, tel que : \$\\Phi\_{verre} = \\theta \\times
    \\Phi\_{incident}\$ avec \$\\theta\$, l'angle d'inclinaison.

-   **Transmittance verre** La valeur de ce coefficient joue sur la
    quantité de flux solaire atteignant le tissu, permettant
    l'échauffement du système. De plus, il est à noter que le verre ne
    possède pas la même valeur de transmittance selon la longueur d'onde
    incidente. Ainsi, une partie du rayonnement est piégée à l'intérieur
    du dessalinisateur, ce qui favorise l'élévation de température. Ce
    phénomène est appelé effet de serre. Cet effet permet d\'augmenter
    la différence de température entre la face intérieure de la vitre et
    l'espace entre celle-ci et le tissu, afin d'optimiser un maximum les
    résultats de notre système. Alors, il est préférable d'étudier la
    transmittance du verre avant de le placer dans notre système.

-   **Environnement : vitesse du vent** Le paramètre le plus important à
    prendre en compte lors de la modélisation est le vent. En effet, ce
    dernier impacte la valeur du coefficient d'échange convecto-radiatif
    entre le verre et l'extérieur. Ainsi, pour étudier le comportement
    du système dans tous les cas de figures, il serait intéressant de
    noter le comportement de la valeur du coefficient d'échange
    convecto-radiatif avec la vitesse du vent.

-   **Température ambiante** Selon la température ambiante insérée lors
    de la modélisation, les résultats attendues sur le débit d\'eau pure
    obtenu varient entre eux. En effet, une différence de température
    ambiante impacterait les valeurs des échanges thermiques, notamment
    entre l\'extérieur et les composants du système.

### Conclusions tirées sur le cas d\'usage

```{=html}
<p class="alinea">
A la lumière du travail réalisé dans le livrable 3, le cas d'usage choisi s'est avéré problématique sur certains points : 
```
-   Il peut paraître incohérent de s\'efforcer à construire un système
    peu énergivore, générant peu de déchets, alors que nos modes de vie
    occidentaux sont complétement en décalage avec cette idée. Faut-il
    prioriser l\'accès à l\'eau en quantités suffisantes quitte à faire
    des compromis sur les impacts environnementaux? La démarche semble
    alors inadaptée pour répondre à un besoin essentiel comme celui de
    l\'eau douce.

-   les faibles (voire très faibles) rendements obtenus vont être un
    frein majeur au développement de notre projet. En effet, ces
    derniers ne permettent pas d\'obtenir la quantité d\'eau minimale
    nécessaire pour la vie d\'un foyer.

-   les rendements sont fortement liés aux conditions climatiques, ce
    qui est problématique dans le cadre d\'un usage quotidien.

-   Rajouter étude sur nuages au nigeria.

```{=html}
<p class="alinea">
Face aux problèmes décrits, une autre proposition de cas d'usage nous a paru plus cohérente et adaptée à notre système : utliser l'eau obtenue par notre système pour l'entretient des espaces verts des communes (ou villes à plus grande échelle) proches de la mer. Ce cas d'usage répond aux problématiques soulevées précédemment. En effet, il est pertinent de développer ce système en France. Il permettra de répondre aux vagues de chaleurs induisant des pénuries d'eau, de plus en plus fréquentes. On répond aussi aux problèmes des rendements faibles puisque l'eau pourra être stockée et ne servira que de "système d'appoint", utilisée uniquement en cas de période de stress hydrique. A grande échelle, ce système pourrait s'avérer être déclencheur d'un changement de paradigme sur l'utilisation de nos ressources en eau, sujet qui deviendra sans doute capital dans les années à venir.
```
