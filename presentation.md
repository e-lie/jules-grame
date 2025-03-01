# SuperTuning

### Dispositif de musique acousmatique pour le live hybride multicanal

## Présentation

Le projet SuperTuning désigne pour moi le développement croisé d'un dispositif de live acousmatique multiphonique et d'une proposition musicale en évolution continue. Basé sur le logiciel SuperCollider, il rassemble mes recherches personnelles en synthèse sonore, composition assistée par ordinateur ainsi que des réflexions d’interaction homme machine. Je développe ce dispositif autour d'un contrôleur et imagine des interactions expressives que je tente de mettre au service de mes intuitions pour articuler un discours musical singulier. L'intention que je poursuis depuis quelques année est d'envisager l’ordinateur comme un instrument de musique acousmatique, ce qui ne va pas forcément de soi au regard des techniques traditionnelles employées dans ce champ de recherche musicale.

Le dispositif se construit dans un premier temps autour de nombreux enregistrements sonores et bandes composées issues de ma pratique de composition électroacoustique plus classique. Il est également inspiré par les recherches en informatique et les propositions musicales d'auteurs et compositeurs comme Robert Schwartz et Curtis Roads dont j'apprécie notamment la précision sonore. Il se nourrit enfin de la rencontre, par l'intermédiaire de Raphaël Formant, du Cookie Collectif qui rassemble des praticiens d'art génératif live et notamment de livecoding musical. À la sortie de ma formation RIM à Saint-Étienne, cette rencontre m'a permis d’approfondir divers aspects techniques de l’informatique musicale et d'explorer en particulier les possibilités du livecoding.


 J'appréhende le livecoding, pratique somme toute encore peu courante et visible, comme une forme de lutherie numérique à l’aide de langages informatiques. Issue de ces hybridations, SuperTuning aborde la composition acousmatique en invitant des techniques informatiques assez récentes et ouvertes à la dimension live: j’ai décidé d’y injecter progressivement tout ce que j'expérimente avec SuperCollider en l’orientant vers une proposition musicale inspirée par la musique acousmatique.
 
L'enjeu dans ma recherche avec cet instrument consiste à trouver des points de rencontre entre des machines de synthèse sonore, exprimées via le langage de SuperCollider et les enregistrements que je fait au micro.

Beaucoups de SynthDef (synthétiseur dans SC) du live on été conçus dans le but de recréer des sons concrets uniquement à partir de synthèse. 

Avec tout ce soutien, je me suis lancé dans la conception de mon premier live : SuperTuning.





Le travail de nathan ho m'intéresse beaucoup par sa radicalité, il utilise uniquement SuperCollider pour composer.

A travers ces articles, qu’il poste sur un site web, il décrit ces recherches et comment il a abouti à certains résultats souhaités, et sur sa chaine youtube il montre son côté intuitif, ces “mécanismes” de design sonore. Ce duo créatif à grandement influencé la conception de SuperTuning.


La notion de paysage sonore est aussi présente dans mon imaginaire de composition.

Recréer des espaces fictifs par le son comme par exemple dans sud de Jean-Claude Risset qui finissent par se métamorphoser en sons totalement synthétiques.

Il s’agit pour moi d’aller chercher les frontières, jouer avec la perception autour du concret/synthétique.

Bien que le live soit sectionné en plusieurs parties, il est imaginé comme une longue continuité.

Plusieurs trames s'enchevêtrent de manière à garder une vitesse, une attention narrative.

Le travail de Christian Zanésis dans Les voix de Pierre Schaeffer représente pour moi cette technique de l’attention que les conteur.euse maîtrisent.  

Au sein du cookie collectif, qui fréquente le hackerspace le fuz, il y a une présence de la culture hacker.


On s’arrange ses propres outils, on ressoude, on répare, on utilise des logiciels libres, on participe au développement d’autres projets lorsqu'on les utilise,..

Cet environnement à influencé certains aspects de la création de SuperTuning, qui est conçu entièrement sur arch linux, avec SC et dont le code est disponible sur la plateforme GitHub. https://github.com/Jules-dejardin/code_d-luges_live

C’est un dispositif bernard l’hermite, je suis la chair qui transporte un dispositif qui me conviens trouver dans un environnement traverser.

L’aspect multicanal est apparu en développant avec mon camarade de jeu Elie Gavoty, un système son 16.1.

Nous formons le duo de musique FRONSSONS ʕ •`ᴥ•´ʔ, dans lequel j’utilise aussi SuperTuning un peu modifié et joué différemment.

Ce premier système nous a permis d’expérimenter le multicanal.

Je lui envoyais 4 pistes qu’il répartissait ensuite dans sur les 16 canaux, grâce au VST ReaSurroundPan. A présent, Elie possède un système octophonique sur lequel nous jouons directement avec chacun 8 canaux. 

## La composition + dispositif || y’a quoi sous l’capot ?

1. Composition

Le projet est structuré par ce que je nomme des tableaux. Un tableau par toujours d’une image qui m’évoque une étape du discours narratif. La narration est assez importante au moment de jouer le dispositif. Elle décide de l'état émotionnel dans lequel je vais jouer et aussi va influencer le choix des éléments sonores: les “couleurs”, le ton, les grains, les timbres… 
Je manipule en live des sons et des articulations que l’on retrouve dans le répertoire acousmatique. Il n’y a pas de rythme ou de mélodie qui joue avec le langage tonal. Lorsqu’une mélodie apparaît c’est de manière anecdotique, pour faire penser à ce qu’on as habitude d'écouter plutôt que de jouer avec ces règles. La radio joue aussi le rôle d’une fenêtre sur le familier, le proche de nous, elle propose une porte d’entrée identifiable par les personnes n’écoutant pas de musique acousmatique. C’est plus une invitation qu’une affirmation. 
SuperTuning se compose d’unités que je nomme tableau. Chaque tableau à une histoire, une couleur, et comme un réel tableau on peut l'observer les détails dans l’ordre que l’on souhaite. Chaque tableau est improvisé tout en gardant une identité propre. Ce système d’unité me permet de jouer le live de manière souple, l’ordre peut-être différent selon mon état d’esprit et le contexte. Je peux m’installer plus confortablement dans la narration. Je ne souhaite pas me faire coincer par une discursivité dans laquelle je ne me reconnais plus. 
Pour le moment, il y a en tout  5 tableaux :### 

- la radio (intro)
- la forêt
- la chambre
- la mer
- le vent (outro)

qui s’enchaine dans l’ordre cité depuis le derniers concert solo (instants chavirés 19/11/24)

2. Dispositif

Le projet est écrit principalement avec SuperCollider (SC) et pour faciliter certains processus j’utilise Reaper. Au live je dispose de mon ordinateur avec une carte son multicanal, d’une radio vintage et de la fameuse interface MIDI avec beaucoup de potentiomètres (launch control xl).
SC gère la synthèse, la lecture des samples, leurs traitements, la spatialisation ainsi que les patterns. 
Reaper gère deux VST qui sont appliqués à la radio, je ne pouvais plus utiliser VSTPlugin dans SC car cela prenait trop de DSP. Maintenant que cette connexion à été faite, j’envisage d’utiliser Reaper comme station de mix multicanal. 
La structure du code est représentée en partie dans le mapping que j’ai choisi pour le contrôleur.

IMAGE (controleur)

Ce contrôleur me permet d’avoir plusieurs pages MIDI. Chaque page est un tableau, j’ai accès au même type de contrôle pour chaque partie mais varié, modulé. J’ai le sentiment que cette structure commune aux différentes parties facilite les transitions entre les différents états et tisse plus facilement des liens entre elles.
J’ai accès à cinq types d’actions
système de sample
La partie “samples” sur l’image est une zone de trigger d’objets sonores que j’ai choisi. Il y a plusieurs variations du même sample choisies aléatoirement par SC. 
Chaînage d’effets
Patterns + modulations
Les “mélodies” font partie de la catégorie patterns, ce sont de long fichier audio que j’ai composé en amont. Hormis cela, les paternes sont des routines qui jouent des enregistrements ou des SynthDefs, souvent en boucles, avec des départs aléatoires. 
VST Delay 
Le delay est jouable pour moi comme un véritable synthétiseur, un instrument.
Volumes des bus 
Pouvoir mixer les différentes sources sonores. 
Radio
	La radio est granulée en temps réel, je peux agir sur le pitch, la taille des grains, la couleur avec un filtre. La radio peut-être freeze, hachuré avec un LFO ou réverbéré. 

IMAGE (Schema archi)

## Mon travail pendant la résidence

### Spatialisation

Où faut-il laisser accès au jeu spatial ? 
où faut-il faire des routine ? 
où faut il figer des plans ? 

Le travail de spatialisation n’est pas quotidiennement aisée. Bien que je puisse avoir accès à deux octophonie dans mon quotidiens (au cons et avec Elie), il est difficile de se focaliser plusieurs jours uniquement sur cet aspect. Prendre le temps de réflexions, d’expérimentation me permet de mieux comprendre ce que manipule. Perpétuellement il faut être multitache et cela implique de négliger certains points. Le projet manque à mes yeux de composition spatiale. Jusqu’à maintenant l’important pour SuperTuning était sa structure de code et son design sonore. Au cours du travail, il me semble avoir mieux domestiquer ces parties, la technique n’est plus un facteur troublant.
Pour le moment, j'aborde la spatialisation surtout avec des routines. Je choisi un parcours pour un type de sons, qui va être joué en boucle. Le mouvement n’est pas toujours très lisible si il y a trop de vitesse par exemple ou si le son se propage trop aléatoirement.

La spatialisation est aussi abordée avec des plans fixes. Inspiré grandement de la pratique de l’acousmonium, il faut simplement décider de là ou se trouve l'élément en fonction de sa place dans la composition de son timbre, de ce qu’il “raconte”. Une de ce que je nomme mélodie est un plan fixe où l’on entend quelqu’un parler et jouer avec de l’eau. Ce tableau est polarisé par l’enregistrement, la personne occupe un espace. Cet ancrage est très fertile il permet d’habiller la situation, de créer aussi une rupture / différence avec ce qui se passe avant et après. 

Finalement il est possible de jouer de l’espace comme tout autre paramètres. Agiter une routine, placer une source, provoquer un changement de trajectoire,...  à l’aide de potentiomètres ou d’autres paramètres. Ce point est le moins exploré dans le projet et est celui qui me donne le plus envie de travailler la spatialisation. Intégrer profondément la notion d’espace aux choix de composition et aux instances de jeu.  
Comment introduire la spatialisation aux mécanismes de jeu déjà présent ?   


