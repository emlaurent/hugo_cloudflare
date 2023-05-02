```{=html}
<html>
```
```{=html}
<style>

h1, h2, h3, h4
    {
      display: block;
    }
    h1{
      font-size : 400%;
      margin: 2%;
      text-align : center;
      text-decoration: underline;
    }
    h2
    {
      font-size : 200%;
      margin:1%;
      text-decoration: underline;
    }
    h3
    {
      font-size : 110%;
      margin: 1%;
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
```{=html}
<p class="alinea">Ce projet s'incrit dans la compréhension de différentes low-tech dont le dessalinisateur solaire. Cette étude a été assigné au groupe GEnEPI 6 et a pour but de développer une production dans un cas d'usage concret pouvant venir en aide à une population. Ainsi, ce projet a suivi différentes étapes allant de l'identification des besoins jusqu'à la modélisation du système en passant par le choix du cas d'usage et la validation du système dans ce cadre là. Cette expérience a été riche en apprentissages, une partie de cette synthèse sera donc consacrée à ces enseignements.  
```
```{=html}
<h3>I- Identification des besoins </h3>
```
```{=html}
<p class="alinea">Aujourd'hui, des pressions s'établissent autour de l'accès à l'eau potable. Il s'agit ici de définir les frontières de cet enjeu dans le but de justifier la raison d'être du dessalinisateur au sein de la société.
L'eau est un besoin vital pour l'Homme, tant pour la consommation que dans la vie quotidienne : douches, lavage des aliments, arrosage des plantes, abreuvage des animaux... Les inégalités autour de l'accès à cette eau augmentent à l'instar des effets du réchauffement climatique et des pollutions anthropiques : les sources s'assèchent, les eaux douces restantes sont polluées et ce sont les plus démunis, alors que ce sont les moins responsables, qui en sont les plus grandes victimes.
```
```{=html}
<p class="alinea">Les sources naturelles en eau ne suffisent plus : la nécessité de trouver des alternatives et par dessus tout d'en trouver pour les minorités qui en souffrent est urgente.  
```
```{=html}
<h3>II- Cas d'usage envisageable </h3>
```
```{=html}
<p class="alinea">Le dimensionnement et l'étude d'un projet de dessalinisation solaire low-tech nécessite la définition d'un contexte d'utilisation. En effet, les spécificités d'un dessalinisateur conditionnent sa viablilité afin de répondre aux besoins précédemment évoqués.
```
```{=html}
<p class="alinea">Après un temps de réflexion, il a été imaginé d'ancrer le système technique au sein d'un village très pauvre sur une côte et situé dans une zone ensoleillée.
```
```{=html}
<p class="alinea">En effet, les habitants d'un tel village n'auraient pas d'accès direct à un fournisseur d'eau potable et pourraient s'approvisionner en eau plus facilement.
```
(Nous avons détaillé notre réflexion dans le [Livrable
2](https://pad.lamyne.org/7rxHkNOAToO-0lNLQ_BVow?both#Cas-dusage-retenu-village-tr%C3%A8s-pauvre-sur-une-c%C3%B4te-et-situ%C3%A9-dans-une-zone-ensoleill%C3%A9e))

```{=html}
<h3>III- Dessalinisateur Watercone® </h3>
```
```{=html}
<img style="display: block; margin: 0 auto;" src="https://hot-objects.liiib.re/pad-lamyne-org/uploads/1b3cda5f-11d8-4b5a-a675-d99dab468df1.png" width="40%">
```
```{=html}
<h4> Figure 1: Dessalinisateur Watercone® </h4>
```
```{=html}
<p class="alinea">Il n'est composé que d'un couvercle transparent et d'un réservoir de couleur noire d'un diamètre d'environ 70 cm dans lequel l'eau salée est placée. La couleur noire de ce dernier permet une meilleure absorption du rayonnement solaire à l'origine du chauffage de l'eau salée. Ce réchauffement provoque l'évaporation de l'eau qui est ainsi séparée des molécules de sel et donc adoucie. Lorsque cette vapeur atteint la paroi du couvercle, plus froide, elle se condense et glisse le long du cône jusqu'à une gouttière située à son extrémité basse. Le principal inconvénient de ce système est qu'il nécessite l'intervention d'un opérateur afin de récupérer l'eau condensée à intervalles réguliers, en renversant le contenu du couvercle dans une bouteille. Un autre point négatif est qu'il ne produit pas assez d'eau par jour pour couvrir les besoins quotidiens d'une personne. De plus, l'eau obtenue ne peut pas être considérée comme potable (un petit peu comme l'eau de pluie) car elle ne contient pas les sels minéraux nécessaires à la consommation humaine. Une consommation régulière d'une telle eau pourrait engendrer des carrences et donc nuire à la santé du consommateur.
```
```{=html}
<p class="alinea">Dans la suite de cette synthèse, pour simplifier la modélisation et la réalisation, le dessalinisateur sera constitué d'un reservoir circulaire avec une simple feuille de plastique en guise de couvercle.
```
![](https://hot-objects.liiib.re/pad-lamyne-org/uploads/4f1fee45-8d35-44c0-b6da-5a9ad6c931c1.PNG)

```{=html}
<h4> Figure 2: Dessalinisateur modélisé </h4>
```
```{=html}
<h3>IV- Modélisation Watercone® </h3>
![Uploading file..._9b843tjlq]()
```
```{=html}
<p class="alinea">Dans le but de connaitre le rendement maximal du système envisagé, il faut réaliser une étude des transferts thermiques. Pour simplifier la compréhension et la modélisation, plusieurs hypothèses simplificatrices ont été faites ainsi qu'un schéma électrique équivalent. Ce schéma permet de décrire les transferts thermiques en faisant une analogie à l'électricité. Les différents échanges étant modélisés par des résistances, avec des expressions physique des flux qui se ramène à une loi d’Ohm transposée aux transfert thermique :
A la place de : 
 U=RI
Les flux s’expriment comme :
ϕ=(Tc-Tf)/R_eq 
Dans les transferts thermiques, les flux de chaleur décrivent la puissance énergétique échangée entre deux milieux avec une température différente. Plus simplement, il s'agit de la quantité de chaleur qui traverse une surface donnée par unité de temps. Ces flux sont toujours orientés de la source la plus chaude vers la plus froide. 
```
```{=html}
<p class="alinea">Pour simplifier les calculs, de nombreuses hypothèses simplificatrices ont été faites. Celle-ci sont développées dans le troisième livrable de l’étude. Ces hypothèses permettent d’obtenir assez simplement un ordre de grandeur des performances du système. Le schéma thermique équivalent simplifié du watercone® est donc le suivant :  
```
![](https://hot-objects.liiib.re/pad-lamyne-org/uploads/36e955b5-0fd7-4b1e-b44d-cea9feabf1df.png)

```{=html}
<h4> Figure 3: Schéma équivalent du Watercone </h4>
```
```{=html}
<p class="alinea">Les équations décrivant les échanges de ce schéma sont regroupées dans le troisième livrable de l’étude: 
```
[Lien vers le
L3](https://docs.google.com/document/d/1djfi9HZ56lDhMWUiQXvnU2VtN2d6a5YRSYXzQ3n_uXY/edit?usp=sharing)

```{=html}
<p class="alinea">Ces échanges thermiques font appel aux quatre grands modes de transfert thermique qui sont : la conduction, la convection, le rayonnement et le changement de phase. 
```
```{=html}
<p class="alinea">La conduction est un mode de transfert thermique dans lequel la chaleur se déplace à travers un matériau solide sans qu'il y ait de mouvement macroscopique du matériau lui-même. Un exemple de conduction est lorsque vous touchez une poêle chaude, la chaleur se déplace à travers la poêle en métal et dans votre main.
```
```{=html}
<p class="alinea">La convection est un mode de transfert thermique qui implique le déplacement de la chaleur par un fluide, tel que l'air ou l'eau. Cela se produit lorsque le fluide se déplace en raison d'une différence de densité ou de température, transférant ainsi la chaleur d'une région à une autre. Un exemple de convection est la circulation de l'air chaud à l'intérieur d'un four.
```
```{=html}
<p class="alinea">Le rayonnement est un mode de transfert thermique qui se produit lorsque la chaleur est transférée par des ondes électromagnétiques, telles que la lumière. Le rayonnement ne nécessite pas de milieu pour se propager et peut se déplacer à travers le vide. Un exemple de rayonnement est la chaleur que vous ressentez sur votre peau lorsque vous êtes exposé au soleil.
```
```{=html}
<p class="alinea">Les changements de phase sont un mode de transfert thermique qui se produit lorsqu'une substance change d'état physique, par exemple de l'eau liquide à de la vapeur ou de la glace solide à de l'eau liquide. Ces changements de phase se font pour une pression constante à température constante, par exemple l’eau liquide s’évapore à 100°C à pression atmosphérique. Ce n’est pas le cas pour le watercone. Les changements de phase de l’eau, qui sont l’évaporation et la condensation sont un peu plus complexe. 
```
```{=html}
<p class="alinea">L'exemple d'une flaque d'eau peut être pris pour comprendre. Lorsque de l'eau est présente à la surface de la terre sous forme de flaque, les molécules d'eau sont continuellement en mouvement. Certaines molécules d'eau ont suffisamment d'énergie pour rompre les forces intermoléculaires qui les retiennent à la surface de la flaque et passer dans l'air environnant. C’est l’évaporation. L'énergie nécessaire pour rompre les forces intermoléculaires provient de la chaleur de l'environnement environnant. C'est pourquoi l'évaporation est plus rapide dans des conditions chaudes et sèches.
Lorsque les molécules d'eau s'évaporent de la surface de la flaque, elles se dispersent dans l'air environnant sous forme de vapeur d'eau. La quantité de vapeur d'eau que l'air peut contenir dépend de sa température et de sa pression. Lorsque l'air est saturé de vapeur d'eau, il ne peut plus absorber d'eau supplémentaire par évaporation.
Au contact d’une source froide la vapeur d'eau se refroidit, les molécules ralentissent et se rapprochent les unes des autres. Elles finissent par se rassembler en gouttelettes d'eau liquide, c’est la condensation. 
```
```{=html}
<p class="alinea">Pour améliorer le watercone, il faut donc trouver les conditions idéales pour maximiser les phénomènes d’évaporation et de condensation.
```
```{=html}
<p class="alinea">Ces conditions s’obtiennent en étudiant l’influence des paramètres thermiques. Cela a permis de définir les paramètres optimaux permettant le dimensionnement du watercône. Les paramètres principaux sont donc : 
*   Les conditions extérieures, avec le jour de l’année considéré avec une influence sur la quantité d’énergie disponible au récepteur, la vitesse du vent favorisant le refroidissement de la vapeur pour la condenser, mais aussi les températures initiales.
```
-   L'émissivité du récepteur, c'est-à-dire la quantité d'énergie qu'il
    peut absorber par rapport à celle qu'il reçoit

-   La taille du système, ainsi que la quantité d'eau initiale qui doit
    être ajustée pour maximiser la production.

```{=html}
<p class="alinea">Cette étude a permis d’obtenir les paramètres suivants :
```
![](https://hot-objects.liiib.re/pad-lamyne-org/uploads/86f224f7-0e54-4b10-962b-93a3cced5cba.PNG)

```{=html}
<h4> Figure 4: Paramètres optimaux </h4>
```
```{=html}
<p class="alinea">Ces paramètres permettent alors d’obtenir les chiffres suivants, avec un rendement maximal légèrment supérieur à 40 %, pour une masse d’eau produite de 45.6 Kg/ jour, soit environ 3.63 L/(jour . m²).
```
```{=html}
<p class="alinea">Néanmoins il est important de rappeler que ces valeurs sont seulement des ordres de grandeurs maximiser par de nombreuses hypothèses simplificatrices. Par exemple la prise en considération des nuages influencerait de manière significative les résultats. 
```
```{=html}
<p class="alinea">Ce modèle théorique a été validé grâce à un prototype construit à l'aide de matériaux de récupération. Cette expérience n'a pas permis de confirmer le rendement du dessalinisateur mais a permis de valider un paramètre géométrique important pour la modélisation. Il est possible de trouver plus d'informations sur l'expérience sur le document suivant :   
```
[Lien vers le
L3](https://docs.google.com/document/d/1djfi9HZ56lDhMWUiQXvnU2VtN2d6a5YRSYXzQ3n_uXY/edit#heading=h.m6mtrrq92qql)

```{=html}
<h3>V- Validation du cas d'usage du dessalinisateur </h3>
```
```{=html}
<p class="alinea">Le Watercone ne semble pas être un idéal d'utilisation dans ce cas d'usage.
```
```{=html}
<p class="alinea">L'eau produite grâce au Watercone® se rapproche en effet plus d'une eau distillée or une telle eau ne peut pas être bue régulièrement. Sa consommation régulière engendrerait des carrences de certains minéraux, le corps pourrait à terme se décharger en minéraux ce qui aurait des conséquences sanitaires importantes.
```
```{=html}
<p class="alinea">En général, les systèmes low-tech sont très peu viables.
Il y a différents moyens de dessaliniser de l'eau salée, que ce soit en utilisant des systèmes techniques low-tech ou bien high-tech. Ces derniers, comme le principe d'osmose inverse qui impose le passage de l'eau à travers une membrane, ou le principe de l'electrodialyse qui utilise un courant électrique pour séparer les ions constituants le sel, ne seront pas détaillés ici car ils ne peuvent pas être des concurrents à notre produit dans le cadre de ce cas d'usage. 
```
```{=html}
<p class="alinea">Dans ce cas, il serait préférable d'utiliser le Watercone® dans un autre cadre, de modifier le cas d'usage. L'usage de l'eau distillée produite grâce au Watercone® pourra être plus intéressant dans un projet pédagogique au sein d'un lycée.er
```
```{=html}
<h3>VI- Retour d'expérience </h3>
```
```{=html}
<p class="alinea">Ce projet a été très riche en découvertes. Nous avons développé des compétences pour rendre notre travail de recherche et de synthèse d'informations plus efficace et plus ciblé. Par exemple, le mot clé "distillateur" propose de biens meilleurs résultats de recherches de publications scientifiques ou d'articles concrets hors du domaine low tech.
```
```{=html}
<p class="alinea">Nous avons pu nous rendre compte de la complexité d'intégrer les technologies low-techs à des cas d'usage concrets. Le dessalinisateur ne semble pas pouvoir produire des quantités utiles pour les individus, et la qualité de l'eau produite est probablement insuffisante pour être considérée comme potable. Dans notre mode de vie actuel, avec les quantités d'eau que nous consommons, il semble donc difficile d'envisager l'utilisation seule des low-techs. La low-tech est donc plus un état d'esprit à avoir: produire des sytèmes moins énergivores tout en questionnant la nécessité de notre consommation actuelle par rapport à nos besoins.
```
