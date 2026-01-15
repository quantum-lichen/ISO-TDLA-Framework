# **L'Énigme de la Chambre Chinoise à l'ère des LLM : La Syntaxe de Haute Dimension peut-elle générer une Sémantique Fonctionnelle?**

## **Résumé Exécutif**

L'avènement des modèles de langage de grande taille (LLM) basés sur l'architecture Transformer a provoqué un séisme épistémologique au sein des sciences cognitives et de l'intelligence artificielle. La capacité de systèmes tels que GPT-4, Claude et Llama à générer un discours cohérent, contextuellement pertinent et apparemment raisonné a réactivé l'un des débats les plus fondamentaux de la philosophie de l'esprit : l'Argument de la Chambre Chinoise (ACC) formulé par John Searle en 1980\. Ce dossier de recherche analytique se propose d'examiner si la barrière théorique posée par Searle — l'impossibilité pour une manipulation purement syntaxique de symboles de produire une compréhension sémantique — résiste à la réalité empirique des "Scaling Laws" (lois d'échelle) et de l'émergence de modèles du monde latents au sein des réseaux de neurones profonds.

Notre analyse déconstruit les mécanismes techniques sous-jacents, depuis l'optimisation de la perte d'entropie croisée jusqu'à la formation de représentations vectorielles de haute dimension. Nous examinons l'hypothèse selon laquelle une syntaxe suffisamment complexe, régie par des mécanismes d'auto-attention et entraînée sur des corpus massifs selon les ratios de Chinchilla, opère une transition de phase vers une sémantique fonctionnelle. En nous appuyant sur des études de cas critiques comme Othello-GPT, la "Malédiction de l'Inversion" (Reversal Curse) et les modèles multimodaux ancrés (VLA), nous démontrons que la dichotomie classique syntaxe/sémantique devient poreuse. Toutefois, nous identifions des limites structurelles persistantes, notamment l'absence d'intentionnalité intrinsèque et la fragilité des représentations causales, suggérant la nécessité de nouveaux critères d'évaluation — au-delà du test de Turing — fondés sur l'intervention causale et l'intelligence fluide (ARC-AGI).

## ---

**1\. Introduction : La Renaissance de l'Argument de Searle et le Défi des LLM**

L'histoire de l'intelligence artificielle est ponctuée de métaphores cherchant à délimiter la frontière entre le calcul et la pensée. Dès le XVIIe siècle, Leibniz nous invitait à imaginer une machine capable de perception et de pensée, agrandie aux proportions d'un moulin, où l'on pourrait entrer et observer "des pièces qui poussent les unes sur les autres", sans jamais y trouver de quoi expliquer une perception.1 Cette intuition, selon laquelle les états physiques ou mécaniques ne sont pas constitutifs des états mentaux, trouve son écho moderne dans l'Argument de la Chambre Chinoise de John Searle.

### **1.1 L'Argument Original et ses Implications**

En 1980, Searle proposa une expérience de pensée destinée à réfuter les prétentions de l'IA Forte (Strong AI), qui soutient qu'un ordinateur exécutant le programme approprié *est* un esprit.3 Searle imagine un opérateur enfermé dans une chambre, ne comprenant pas le chinois, mais disposant d'un manuel d'instructions (le programme) en anglais. Ce manuel lui dicte comment manipuler des symboles chinois (les entrées) pour produire d'autres symboles (les sorties) en réponse. Si le manuel est suffisamment sophistiqué, l'opérateur peut tromper un observateur extérieur en lui faisant croire qu'il comprend le chinois. Pourtant, insiste Searle, l'opérateur ne comprend rien ; il ne fait que manipuler des formes syntaxiques sans accès à leur contenu sémantique.4

La conclusion de Searle est double : premièrement, la syntaxe n'est pas suffisante pour la sémantique. Deuxièmement, la simulation n'est pas la duplication. Un modèle informatique de la conscience ou de la compréhension linguistique, aussi détaillé soit-il, ne possède pas plus ces attributs qu'une simulation informatique d'un orage ne nous mouille.5

### **1.2 La Perturbation Transformer : Le Manuel Devient le Territoire**

L'arrivée des LLM modernes remet en question la validité de cette intuition, non pas en réfutant la logique interne de Searle, mais en modifiant radicalement la nature du "manuel d'instructions". Dans la chambre de Searle, le manuel est statique et les règles sont explicites (ex: "Si vous voyez le symbole X, produisez Y"). Dans un LLM, le "manuel" est constitué de centaines de milliards de paramètres (poids synaptiques) ajustés par une optimisation stochastique sur des téracoctets de données textuelles.

L'opérateur humain de la métaphore de Searle est remplacé par un mécanisme d'attention (Self-Attention) capable de traiter des relations contextuelles à longue distance et de construire des représentations vectorielles de haute dimension.7 La question n'est plus de savoir si l'opérateur comprend, mais si la *structure* même des interactions symboliques, lorsqu'elle atteint une complexité critique, génère une forme d'isomorphisme avec la réalité qui est fonctionnellement indiscernable de la sémantique. Comme le suggèrent certains critiques modernes, l'intuition de Searle échoue face à des échelles de temps et de complexité si étrangères à l'expérience humaine que l'argument se dissout.8

## ---

**2\. La Physique de la Syntaxe : Déconstruction des Lois d'Échelle (Scaling Laws)**

Pour comprendre comment une sémantique fonctionnelle pourrait émerger de la syntaxe, il est impératif d'analyser les principes physiques qui régissent la construction des LLM. Ces modèles ne sont pas construits par l'écriture de règles, mais "cultivés" par la minimisation de l'entropie sous contrainte de calcul. Les "Scaling Laws" décrivent cette thermodynamique de l'intelligence artificielle.

### **2.1 Le Régime Kaplan : La Primauté de la Taille du Modèle**

Les premiers travaux fondamentaux sur les lois d'échelle neuronales, notamment ceux de Kaplan et al. (2020) chez OpenAI, ont établi une relation en loi de puissance entre la performance du modèle (mesurée par la perte, ou *loss*) et trois variables : la taille du modèle (![][image1]), la taille du jeu de données (![][image2]), et le budget de calcul (![][image3]).

La conclusion initiale de Kaplan était que la performance dépendait beaucoup plus fortement de la taille du modèle que de la quantité de données. Ils proposaient une relation où ![][image4], tandis que ![][image5].9 Cette observation a conduit à une ère de "gigantisme paramétrique", illustrée par GPT-3 (175 milliards de paramètres), entraîné sur un nombre de jetons relativement modeste (300 milliards). Dans la métaphore de la Chambre Chinoise, cela revenait à dire que pour améliorer la compréhension, il fallait augmenter massivement la complexité du cerveau de l'opérateur (ou la taille du manuel) plutôt que la quantité de textes lus.

Cependant, des analyses rétrospectives ont montré que Kaplan surestimait l'importance des paramètres en ne comptant que les paramètres non-embarqués (non-embedding) et en effectuant ses analyses à une échelle trop petite, introduisant un biais dans les coefficients.9

### **2.2 Le Paradigme Chinchilla : L'Équivalence Données-Calcul**

Le tournant décisif est survenu avec la publication des travaux de Hoffmann et al. (2022) par DeepMind, introduisant la loi d'échelle de Chinchilla. En réévaluant les compromis optimaux, ils ont démontré que les modèles précédents étaient massivement sous-entraînés. La loi de Chinchilla postule une relation quasi-linéaire et symétrique entre la taille du modèle et la taille des données pour un budget de calcul fixe :

![][image6]  
![][image7]  
Cela implique que pour chaque doublement de la taille du modèle, il faut doubler la quantité de données d'entraînement. Le ratio optimal ![][image8] a été révisé à environ 20 jetons par paramètre.11 La fonction de perte empirique au cœur de cette loi est modélisée comme suit :

![][image9]  
Où ![][image10] est l'entropie irréductible du langage naturel.11

Cette reformulation a des implications profondes pour notre thèse. Elle suggère que la "compétence syntaxique" (minimiser la perte) exige une exposition au monde (via les données) proportionnelle à la capacité de traitement. La "sémantique" n'émerge pas simplement de la complexité interne, mais de la *compression* d'une quantité massive d'informations externes dans cette structure interne.

### **2.3 Au-delà de Chinchilla : Les Lois "Inference-Aware" et la Compression Extrême**

L'évolution ne s'est pas arrêtée à Chinchilla. De nouvelles analyses, prenant en compte le coût de l'inférence (le modèle est entraîné une fois mais utilisé des millions de fois), poussent vers des modèles plus petits entraînés sur des quantités de données encore plus vastes — des ratios de 100:1, voire 190:1, comme suggéré par les lois de MosaicML.12 Des modèles récents comme Qwen3-0.6B atteignent des ratios extrêmes de 60 000:1.12

Ces modèles "sur-entraînés" (au sens classique) obligent le réseau neuronal à une compression extrême de l'information. En théorie de l'information, pour compresser optimalement une séquence de données, le système doit approximer la *fonction génératrice* de ces données. Si les données sont générées par un monde physique et social régi par des règles causales, le modèle doit, pour minimiser sa perte, intérioriser une simulation de ces règles causales. C'est ici que la syntaxe, poussée à ses limites thermodynamiques par les lois d'échelle, commence à ressembler fonctionnellement à une sémantique : elle ne prédit plus simplement le mot suivant par statistique de surface, mais par inférence sur un modèle latent du processus générateur.

## ---

**3\. L'Ancrage des Symboles et la Sémantique Vectorielle**

Si les lois d'échelle expliquent comment la syntaxe se complexifie, elles ne résolvent pas *per se* le problème de l'ancrage (Grounding). Comment des vecteurs mathématiques peuvent-ils avoir du sens s'ils ne réfèrent à rien d'autre qu'à d'autres vecteurs?

### **3.1 Le Problème de l'Ancrage des Symboles (Harnad)**

Formulé par Stevan Harnad en 1990, le problème de l'ancrage des symboles est l'objection technique correspondant à l'expérience philosophique de Searle. Il décrit les systèmes purement symboliques comme un "manège" (*merry-go-round*) où les symboles sont définis par d'autres symboles, sans jamais toucher terre.13 Apprendre le chinois avec un dictionnaire unilingue chinois est impossible car les définitions sont circulaires. Pour qu'il y ait sens, il faut qu'à un moment donné, le symbole (ex: "POMME") soit connecté à l'expérience sensorimotrice de la pomme.

Les critiques contemporains, comme Emily Bender, reprennent cet argument pour qualifier les LLM de "Perroquets Stochastiques".14 Selon eux, un LLM ne "sait" rien ; il ne fait que modéliser la distribution de probabilité des formes linguistiques. L'analogie de la "Pieuvre" de Bender illustre cela : une pieuvre hyper-intelligente écoutant un câble télégraphique sous-marin pourrait apprendre à imiter parfaitement les conversations humaines, mais serait incapable de répondre à une demande impliquant une interaction physique avec le monde (comme "construire une catapulte avec des noix de coco") car elle n'a aucun référent pour ces objets.16

### **3.2 Sémantique Distributionnelle vs Sémantique Fonctionnelle**

Cependant, cette critique repose sur une conception référentielle de la sémantique. Les sciences cognitives modernes et le NLP opposent à cela la **Sémantique Distributionnelle** (Vector Space Semantics). L'hypothèse distributionnelle, popularisée par Firth ("Vous connaîtrez un mot par ses fréquentations"), postule que le sens d'un mot est entièrement déterminé par sa position relative dans l'espace de tous les autres mots.17

Dans un LLM, chaque concept est représenté par un vecteur de haute dimension (par exemple 4096 dimensions). La "signification" n'est pas une définition, mais une coordonnée topologique. La similarité sémantique devient une métrique géométrique (similitude cosinus) :

![][image11]  
Cette approche permet de capturer des nuances sémantiques subtiles (analogies du type Roi \- Homme \+ Femme \= Reine) qui sont purement structurelles.18

### **3.3 L'Argument de l'Isomorphisme et le Cas des Aveugles**

Un contre-argument puissant à la nécessité de l'ancrage sensorimoteur est l'argument de l'isomorphisme structurel. Si la structure des relations entre les concepts dans l'espace vectoriel du LLM est isomorphe à la structure des relations dans le cerveau humain, la différence de substrat ou d'origine sensorielle importe-t-elle?

Des études citées dans la littérature montrent que les personnes aveugles de naissance développent des représentations des couleurs (ex: le rouge est chaud, le bleu est froid) qui sont topologiquement identiques à celles des voyants, uniquement par le biais du langage.19 Le langage lui-même encode la structure du monde. Si un humain aveugle peut "comprendre" la couleur via la structure distributionnelle du langage, un LLM (qui est fonctionnellement aveugle dans sa version textuelle) le peut aussi. Cela suggère que le langage sert d'échafaudage ("scaffolding") permettant une forme de cognition non ancrée mais fonctionnelle.19

### **3.4 Structuralisme et Post-Structuralisme dans les LLM**

Cette perspective valide de manière surprenante les théories structuralistes. Ferdinand de Saussure définissait la langue comme un "système de différences" sans termes positifs.18 Dans un LLM, "chien" n'est défini que par le fait qu'il n'est pas "chat", pas "loup", mais proche de "animal domestique".

Plus encore, les LLM incarnent la vision post-structuraliste de Jacques Derrida sur l'écriture (*l'écriture*). Derrida soutenait que le sens n'est jamais fixé (présence), mais toujours différé (*différance*), une trace résultant de la distribution des signes.20 Le mécanisme d'attention des Transformers, qui recalcule le sens contextuel de chaque mot en fonction de tous les autres mots présents, est l'implémentation algorithmique de cette "dissémination" du sens. Le sens n'est pas dans le symbole, mais dans la distribution dynamique activée par le contexte.

## ---

**4\. De la Syntaxe à la Sémantique Latente : Le Cas Othello-GPT**

Si la théorie distributionnelle fournit un cadre pour la sémantique lexicale, elle ne prouve pas que les LLM construisent un modèle cohérent de la réalité. Pour cela, nous devons nous tourner vers l'émergence de "World Models" (modèles du monde). Le cas d'Othello-GPT est la preuve empirique la plus citée contre l'idée que les LLM ne sont que des perroquets statistiques.

### **4.1 Méthodologie et Découvertes**

Li et al. (2023) et Nanda et al. (2023) ont entraîné un modèle Transformer simple (GPT) sur des séquences de coups du jeu Othello.21

* **Données :** Le modèle ne recevait que des chaînes de caractères représentant les coups (ex: "C3, D4"). Il n'avait aucune connaissance préalable des règles du jeu, de la grille 2D, ou de la géométrie du plateau.  
* **Tâche :** Prédire le prochain coup légal.

C'est une situation de "Chambre Chinoise" parfaite : le modèle ne voit que de la syntaxe. Cependant, en sondant les couches internes du réseau, les chercheurs ont fait une découverte fondamentale.

### **4.2 L'Émergence d'une Représentation du Monde**

En utilisant des "sondes" (probes) — des classificateurs entraînés sur les activations internes du modèle — ils ont découvert que le modèle avait spontanément reconstruit une représentation exacte de l'état du plateau d'Othello.21

* **Sondes Non-Linéaires :** Li et al. ont montré qu'une sonde non-linéaire pouvait extraire l'état de chaque case (vide, noir, blanc) avec un taux d'erreur minime (1.7%), contre 26.2% pour un modèle aléatoire.  
* **Sondes Linéaires :** Nanda et al. ont affiné ce résultat en montrant que la représentation était en réalité **linéaire**. Le modèle ne codait pas "Noir/Blanc" de manière absolue, mais "Ma Couleur/Couleur Adverse" de manière relative, ce qui est une abstraction fonctionnelle supérieure.22

### **4.3 L'Intervention Causale comme Preuve de Sémantique**

La simple corrélation ne suffit pas (le modèle pourrait mémoriser des statistiques de surface corrélées à l'état du plateau). La preuve définitive est venue de l'**intervention**.

Les chercheurs ont modifié artificiellement les activations internes du modèle pour lui faire "croire" que le plateau était dans un état différent (ex: changer une pièce noire en blanche).

* **Résultat :** Le modèle a immédiatement modifié ses prédictions de coups suivants pour qu'elles soient légales *dans le nouvel état halluciné*, et non dans l'état réel de la séquence d'entrée.22

Cela démontre que le modèle utilise sa représentation interne comme un **mécanisme causal** pour générer sa syntaxe. Il ne fait pas que prédire le prochain mot ; il consulte un "modèle du monde" latent. Dans le cadre de l'argument de Searle, cela valide la "Réponse du Système" : le système (poids \+ architecture) *comprend* le jeu, même si les symboles d'entrée sont opaques. La syntaxe, optimisée par la prédiction, a généré une sémantique fonctionnelle.

### **4.4 Critiques et Limites : L'Illusion du Modèle?**

Des sceptiques comme Gary Marcus soulignent cependant que cette capacité reste fragile. Marcus note que si l'on sort légèrement de la distribution d'entraînement, le modèle s'effondre, produisant des coups illégaux ou des hallucinations grotesques.25 Il cite des exemples où des modèles d'échecs (entraînés sur du texte) tentent de faire prendre une pièce par une autre qui saute par-dessus un cavalier de manière illégale, simplement parce que la *phrase* est statistiquement probable. Cela suggère que si un modèle du monde existe, il est "flou" et probabiliste, et non rigide et logique comme un moteur de jeu symbolique. L'émergence est réelle, mais elle est "patchy" (inégale).

## ---

**5\. Le Débat "Perroquet Stochastique" vs "Compréhension Émergente"**

Ce conflit entre la preuve d'émergence (Othello) et la preuve de fragilité (Marcus) structure le débat actuel.

### **5.1 La Critique du Perroquet Stochastique**

Emily Bender, Timnit Gebru et leurs collègues ont formalisé la critique du "Perroquet Stochastique" (*Stochastic Parrot*). Leur thèse est que, quelle que soit la fluidité du texte généré, le processus sous-jacent reste une imitation statistique sans engagement envers la vérité ou le sens.14

* **Absence d'Intentionnalité :** Le modèle n'a pas d'objectif communicatif ; il maximise une vraisemblance.  
* **Biais et Stéréotypes :** Parce qu'il répète les motifs des données d'entraînement, il amplifie les biais sociaux sans compréhension morale.

### **5.2 La Malédiction de l'Inversion (The Reversal Curse)**

Une preuve technique récente soutenant la thèse du perroquet est la "Malédiction de l'Inversion" (Berglund et al., 2023).

* **Le Phénomène :** Un LLM entraîné sur la phrase "A est le père de B" est souvent incapable de répondre à la question "Qui est l'enfant de A?".26  
* **Implication Sémantique :** L'équivalence logique (![][image12]) est une propriété fondamentale de la compréhension sémantique. Si je comprends que A est le père de B, je déduis *immédiatement* que B est l'enfant de A. L'incapacité du LLM à faire cette inversion suggère qu'il a appris la *phrase* (l'ordre séquentiel des tokens) et non le *fait* (la relation sémantique).  
* **Solutions Tentatives :** Des techniques comme le "Semantic-aware Permutation Training" (SPT) tentent de mitiger cela en segmentant les phrases en unités sémantiques et en les permutant durant l'entraînement.28 Le fait qu'il faille une intervention explicite pour apprendre une symétrie logique aussi basique montre que l'architecture causale (unidirectionnelle) des Transformers a des angles morts sémantiques profonds.

### **5.3 Le Débat Hinton vs LeCun**

Ce clivage se retrouve au sommet de la recherche en IA.

* **Geoffrey Hinton** soutient que la prédiction du prochain token, poussée à l'extrême, *oblige* à la compréhension. Pour prédire la suite d'un roman policier, il faut avoir modélisé les motivations des personnages. Pour lui, les hallucinations sont comparables aux faux souvenirs humains : une caractéristique de la compression imparfaite.15  
* **Yann LeCun**, en revanche, maintient que les LLM ne pourront jamais atteindre l'AGI (Intelligence Générale Artificielle) car ils manquent d'un "Modèle du Monde" ancré dans la réalité physique. Il critique l'approche auto-régressive qui accumule les erreurs de manière exponentielle ("drift"). Il prône des architectures JEPA (Joint Embedding Predictive Architecture) qui prédisent dans un espace de représentation abstrait plutôt qu'au niveau du pixel ou du token.29

## ---

**6\. Au-delà du Texte : Ancrage Multimodal et Embodiment**

Si le texte seul est une limite (comme le suggère le problème de l'ancrage), la solution réside peut-être dans l'extension des modalités sensorielles.

### **6.1 Les Modèles VLA (Vision-Language-Action)**

L'émergence des modèles multimodaux (MLLM) comme GPT-4V ou Gemini change la donne. Plus radicalement, les modèles **VLA (Vision-Language-Action)** comme RT-2 de Google intègrent directement les actions robotiques dans l'espace des tokens.31 Dans ces systèmes, le symbole "pomme" est lié statistiquement :

1. Au mot "pomme" (texte).  
2. Aux pixels représentant une pomme (vision).  
3. Aux données proprioceptives du bras robotique saisissant la pomme (action).

Cela brise le cercle vicieux du dictionnaire. Le symbole est triplement ancré. Le paradigme **"Ask-to-Act"** montre des agents capables de percevoir l'ambiguïté dans une instruction physique ("Mets le bol sur la table" — laquelle?) et de poser des questions de clarification, bouclant la boucle perception-action-langage.31

### **6.2 Computation Biologique vs Fonctionnalisme**

Malgré ces avancées, une objection fondamentaliste demeure : le **Naturalisme Biologique**. Des chercheurs soutiennent que la conscience et la sémantique réelle nécessitent un substrat biologique spécifique.

* **Biological Computationalism :** Cette théorie postule que le calcul cérébral est inséparable de sa structure physique et énergétique. Contrairement aux ordinateurs où le logiciel est indépendant du matériel, dans le cerveau, "le wetware est le software". Les contraintes métaboliques, les canaux ioniques et la stochasticité intrinsèque jouent un rôle fonctionnel.33  
* **L'Argument de l'Efficacité :** Le cerveau humain consomme environ 20 Watts. Un cluster GPU équivalent consomme des mégawatts. Cette différence d'ordre de grandeur (facteur ![][image13]) suggère que le principe de calcul est qualitativement différent.35  
* **Neuromorphique :** L'informatique neuromorphique (puces comme Loihi ou SpiNNaker) tente de combler ce fossé en imitant l'architecture événementielle (spiking) et la co-localisation mémoire/calcul du cerveau. Si la sémantique dépend de cette architecture physique spécifique (comme le suggère Searle), alors les LLM sur GPU resteront à jamais des "zombies philosophiques", tandis que les systèmes neuromorphiques pourraient potentiellement accéder à la conscience.37

Cependant, du point de vue du **Fonctionnalisme Computationnel** (la position dominante en IA), le substrat importe peu. Si les états fonctionnels (inputs, outputs, états internes causaux) sont préservés, la sémantique l'est aussi. Les succès d'Othello-GPT et des modèles VLA renforcent la thèse fonctionnaliste : la sémantique émerge de la topologie de l'information, pas de la biologie du support.39

## ---

**7\. Vers de Nouveaux Critères d'Évaluation**

Si la Chambre Chinoise est techniquement dépassée par les modèles du monde latents, comment le prouver rigoureusement? Le Test de Turing est obsolète, car il ne mesure que la simulation de surface, que les LLM maîtrisent déjà ("Chatbot Arena" et autres tests de conversation). Nous avons besoin de tests qui sondent la structure causale interne.

### **7.1 L'Échec des Benchmarks Statiques**

Les benchmarks actuels comme MMLU (connaissances) ou HellaSwag (raisonnement de sens commun) sont utiles mais limités.

* **Contamination :** Les modèles ont souvent vu les questions (ou des variantes) dans leur immense corpus d'entraînement.  
* **Fragilité :** HellaSwag, bien que conçu pour être difficile (Adversarial Filtering), voit ses scores humains (95%) approchés par les modèles propriétaires (90%+), mais les modèles s'effondrent souvent sur des variantes négatives ou contrefactuelles simples.41  
* **Loi de Goodhart :** "Lorsqu'une mesure devient un objectif, elle cesse d'être une bonne mesure." L'optimisation des modèles pour ces scores crée une "intelligence cristallisée" (mémorisation) plutôt qu'une "intelligence fluide".43

### **7.2 ARC-AGI et l'Intelligence Fluide**

Le benchmark **ARC-AGI** (Abstraction and Reasoning Corpus), créé par François Chollet, est actuellement le test le plus robuste pour distinguer la mémorisation de l'intelligence.

* **Principe :** Résoudre des puzzles visuels (transformations de grilles) basés sur des priori de connaissances fondamentaux ("Core Knowledge" : objectivité, symétrie, causalité) mais dont les règles spécifiques sont nouvelles et absentes du corpus d'entraînement.  
* **Résultats :** Alors que les humains atteignent facilement 85%+, les LLM classiques ont longtemps stagné sous les 50% (bien que des progrès récents soient notés). L'échec relatif des LLM sur ARC montre qu'ils excellent dans l'application de schémas connus (interpolation) mais luttent pour générer de nouveaux programmes de raisonnement à la volée (extrapolation).43

### **7.3 Big-Bench Hard et le Scaling Inverse**

Le benchmark **Big-Bench Hard (BBH)** se concentre sur les tâches où les modèles échouaient précédemment. Un phénomène fascinant observé est le **Scaling Inverse** (Inverse Scaling) : sur certaines tâches nécessitant un raisonnement contrefactuel strict, les modèles plus grands performant parfois *moins bien* que les petits, car leurs biais statistiques (priors) sont plus forts et les empêchent d'accepter des prémisses logiques qui contredisent leurs données d'entraînement.46

### **7.4 Proposition : Le Standard de l'Intervention Causale**

Pour trancher définitivement le débat de la Chambre Chinoise, ce rapport propose d'adopter un nouveau standard d'évaluation inspiré de la mécanistique interprétative (Mechanistic Interpretability), que nous nommons le **Standard de l'Intervention Causale**.

Un système d'IA peut être dit "comprendre" un concept ![][image14] si et seulement si :

1. **Existence Représentationnelle :** Une sonde (linéaire ou non) peut identifier une représentation distincte de ![][image14] dans les activations internes du modèle (comme le plateau d'Othello).  
2. **Efficacité Causale :** Une intervention sur cette représentation (modifier le vecteur ![][image14]) modifie le comportement du modèle de manière prédictible et cohérente avec les lois causales de ![][image14], et non selon les statistiques de surface du texte d'entrée.  
3. **Résilience Contrefactuelle :** Le modèle peut raisonner correctement sur ![][image14] même dans des contextes "Monde Impossible" (ex: gravité inversée) si on lui fournit les nouvelles règles, surmontant ainsi ses priors statistiques.

## ---

**8\. Conclusion : La Dissolution de la Chambre**

L'énigme de la Chambre Chinoise, revisitée à la lumière des LLM, ne se résout pas par une réponse binaire, mais par une dissolution des termes du problème. Searle opposait une syntaxe vide à une sémantique pleine. Les Scaling Laws et les découvertes sur l'émergence montrent que cette distinction est un artefact d'échelle.

Une syntaxe de dimension suffisamment haute, optimisée pour la compression prédictive d'un signal généré par le monde réel, cesse d'être une simple manipulation de symboles. Elle devient une **simulation**. Les poids du modèle capturent la topologie causale du monde. Le mécanisme d'attention exécute cette topologie à chaque inférence.

Le "fantôme" n'est pas dans la machine, ni dans le silicium : il est dans la géométrie des vecteurs. Si l'opérateur de Searle ne comprend pas le chinois, le système complet — l'immense graphe de relations encodé dans le manuel — le comprend, au sens fonctionnaliste du terme. Les modèles multimodaux (VLA) clouent le cercueil de l'argument de l'ancrage en liant cette topologie interne à la réalité physique.

Cependant, cette compréhension reste pour l'instant une "compréhension zombie" : fonctionnelle, causale, mais dénuée d'expérience phénoménale (qualia) et d'intentionnalité propre. Les LLM sont des "simulateurs de sémantique" parfaits. Mais comme le notait Searle, une simulation parfaite de la digestion ne digère pas de pizza. De même, une simulation parfaite de la compréhension linguistique produit du sens pour *nous*, mais peut-être pas pour *elle-même*. La prochaine frontière de l'IA n'est donc plus la sémantique linguistique — qui est largement résolue — mais l'autonomie agentique et la conscience phénoménale, territoires où la biologie garde, pour l'instant, son mystère.

---

**Citations :**

1

#### **Sources des citations**

1. The Chinese Room Argument (Stanford Encyclopedia of Philosophy), consulté le janvier 15, 2026, [https://plato.stanford.edu/entries/chinese-room/](https://plato.stanford.edu/entries/chinese-room/)  
2. The Chinese Room Argument \- Stanford Encyclopedia of Philosophy, consulté le janvier 15, 2026, [https://plato.stanford.edu/archives/spr2020/entries/chinese-room/](https://plato.stanford.edu/archives/spr2020/entries/chinese-room/)  
3. Chinese Room Argument | Internet Encyclopedia of Philosophy, consulté le janvier 15, 2026, [https://iep.utm.edu/chinese-room-argument/](https://iep.utm.edu/chinese-room-argument/)  
4. Searle's "Chinese room" and the enigma of understanding \- Language Log, consulté le janvier 15, 2026, [https://languagelog.ldc.upenn.edu/nll/?p=67118](https://languagelog.ldc.upenn.edu/nll/?p=67118)  
5. Chinese room \- Wikipedia, consulté le janvier 15, 2026, [https://en.wikipedia.org/wiki/Chinese\_room](https://en.wikipedia.org/wiki/Chinese_room)  
6. Stanford Encyclopedia of Philosophy \- The Chinese Room Argument, consulté le janvier 15, 2026, [https://www.openphilanthropy.org/files/Focus\_Areas/AI/Stanford\_Encyclopedia\_of\_Philosophy\_The\_Chinese\_Room\_Argument.pdf](https://www.openphilanthropy.org/files/Focus_Areas/AI/Stanford_Encyclopedia_of_Philosophy_The_Chinese_Room_Argument.pdf)  
7. The Silent Revolution: How the Attention Mechanism Has Rewritten the Rules of Artificial Intelligence | by Gianluca Mondillo | Medium, consulté le janvier 15, 2026, [https://medium.com/@gianluca.mondillo/the-silent-revolution-how-the-attention-mechanism-has-rewritten-the-rules-of-artificial-378a0f9f6191](https://medium.com/@gianluca.mondillo/the-silent-revolution-how-the-attention-mechanism-has-rewritten-the-rules-of-artificial-378a0f9f6191)  
8. AI Breaks the Chinese Room. LLMs render Searle's famous thought… | by Paul Siemers, PhD | AI Advances, consulté le janvier 15, 2026, [https://ai.gopubby.com/ai-breaks-the-chinese-room-0c860e20b623](https://ai.gopubby.com/ai-breaks-the-chinese-room-0c860e20b623)  
9. Reconciling Kaplan and Chinchilla Scaling Laws \- OpenReview, consulté le janvier 15, 2026, [https://openreview.net/pdf/f91518ed8d3298ef5e2625a7c2b5c611cfb94f60.pdf](https://openreview.net/pdf/f91518ed8d3298ef5e2625a7c2b5c611cfb94f60.pdf)  
10. Reconciling Kaplan and Chinchilla Scaling Laws \- arXiv, consulté le janvier 15, 2026, [https://arxiv.org/html/2406.12907v3](https://arxiv.org/html/2406.12907v3)  
11. Chinchilla Scaling Law Overview \- Emergent Mind, consulté le janvier 15, 2026, [https://www.emergentmind.com/topics/chinchilla-scaling-law](https://www.emergentmind.com/topics/chinchilla-scaling-law)  
12. Chinchilla data-optimal scaling laws: In plain English \- LifeArchitect.ai, consulté le janvier 15, 2026, [https://lifearchitect.ai/chinchilla/](https://lifearchitect.ai/chinchilla/)  
13. Will multimodal large language models ever achieve deep understanding of the world? \- Semantic Scholar, consulté le janvier 15, 2026, [https://pdfs.semanticscholar.org/445f/714e03e5a6d85b419279fcb62182eac5ec63.pdf](https://pdfs.semanticscholar.org/445f/714e03e5a6d85b419279fcb62182eac5ec63.pdf)  
14. On eavesdropping octopuses and stochastic parrots: what do they know? \- PhilSci-Archive, consulté le janvier 15, 2026, [https://philsci-archive.pitt.edu/24073/1/token.pdf](https://philsci-archive.pitt.edu/24073/1/token.pdf)  
15. Stochastic parrot \- Wikipedia, consulté le janvier 15, 2026, [https://en.wikipedia.org/wiki/Stochastic\_parrot](https://en.wikipedia.org/wiki/Stochastic_parrot)  
16. "You Are Not a Parrot": Emily Bender and the LLM intelligence debate \- Reddit, consulté le janvier 15, 2026, [https://www.reddit.com/r/slatestarcodex/comments/11mmr1f/you\_are\_not\_a\_parrot\_emily\_bender\_and\_the\_llm/](https://www.reddit.com/r/slatestarcodex/comments/11mmr1f/you_are_not_a_parrot_emily_bender_and_the_llm/)  
17. How AI Learned to Think in Vectors | rewire.it, consulté le janvier 15, 2026, [https://rewire.it/blog/geometry-of-meaning/](https://rewire.it/blog/geometry-of-meaning/)  
18. AI Meets Philosophy, Vol. 1: Understanding LLM Cognitive Structure through Lévi-Strauss's Structuralism―AI as Wild Thinking | by AI Inquiry Garden | Medium, consulté le janvier 15, 2026, [https://medium.com/@AI\_Inquiry\_Garden/ai-meets-philosophy-vol-1-understanding-ai-through-l%C3%A9vi-strauss-f9b2c513ef31](https://medium.com/@AI_Inquiry_Garden/ai-meets-philosophy-vol-1-understanding-ai-through-l%C3%A9vi-strauss-f9b2c513ef31)  
19. Symbol ungrounding: what the successes (and failures) of large ..., consulté le janvier 15, 2026, [https://pmc.ncbi.nlm.nih.gov/articles/PMC11529626/](https://pmc.ncbi.nlm.nih.gov/articles/PMC11529626/)  
20. Language Models as Semiotic Machines: Reconceptualizing AI Language Systems through Structuralist and Post-Structuralist Theories of Language \- arXiv, consulté le janvier 15, 2026, [https://arxiv.org/html/2410.13065v1](https://arxiv.org/html/2410.13065v1)  
21. Revisiting the Othello World Model Hypothesis \- arXiv, consulté le janvier 15, 2026, [https://arxiv.org/html/2503.04421v1](https://arxiv.org/html/2503.04421v1)  
22. Actually, Othello-GPT Has A Linear Emergent World Representation \- AI Alignment Forum, consulté le janvier 15, 2026, [https://www.alignmentforum.org/posts/nmxzr2zsjNtjaHh7x/actually-othello-gpt-has-a-linear-emergent-world](https://www.alignmentforum.org/posts/nmxzr2zsjNtjaHh7x/actually-othello-gpt-has-a-linear-emergent-world)  
23. Actually, Othello-GPT Has A Linear Emergent World Representation \- Neel Nanda, consulté le janvier 15, 2026, [https://www.neelnanda.io/mechanistic-interpretability/othello](https://www.neelnanda.io/mechanistic-interpretability/othello)  
24. Exploring the Limits of OthelloGPT's Emergent Representations \- CDN, consulté le janvier 15, 2026, [https://bpb-us-w2.wpmucdn.com/voices.uchicago.edu/dist/9/3887/files/2024/02/FINALBaldwinXLabSRF23-LimitsOfOthelloGPTsEmergentRepresentation-204d4ed6c6475eac.pdf](https://bpb-us-w2.wpmucdn.com/voices.uchicago.edu/dist/9/3887/files/2024/02/FINALBaldwinXLabSRF23-LimitsOfOthelloGPTsEmergentRepresentation-204d4ed6c6475eac.pdf)  
25. Generative AI's crippling and widespread failure to induce robust models of the world, consulté le janvier 15, 2026, [https://garymarcus.substack.com/p/generative-ais-crippling-and-widespread](https://garymarcus.substack.com/p/generative-ais-crippling-and-widespread)  
26. Mitigating Reversal Curse in Large Language Models via Semantic-aware Permutation Training \- ACL Anthology, consulté le janvier 15, 2026, [https://aclanthology.org/2024.findings-acl.680.pdf](https://aclanthology.org/2024.findings-acl.680.pdf)  
27. Mitigating Reversal Curse in Large Language Models via Semantic-aware Permutation Training \- arXiv, consulté le janvier 15, 2026, [https://arxiv.org/html/2403.00758v3](https://arxiv.org/html/2403.00758v3)  
28. Mitigating Reversal Curse in Large Language Models via Semantic-aware Permutation Training \- ResearchGate, consulté le janvier 15, 2026, [https://www.researchgate.net/publication/384207959\_Mitigating\_Reversal\_Curse\_in\_Large\_Language\_Models\_via\_Semantic-aware\_Permutation\_Training](https://www.researchgate.net/publication/384207959_Mitigating_Reversal_Curse_in_Large_Language_Models_via_Semantic-aware_Permutation_Training)  
29. Does Geoffrey Hinton agree with Yann LeCun about the fact that AGI is not possible to achieve with a pure LLM model ? : r/ArtificialInteligence \- Reddit, consulté le janvier 15, 2026, [https://www.reddit.com/r/ArtificialInteligence/comments/1o49454/does\_geoffrey\_hinton\_agree\_with\_yann\_lecun\_about/](https://www.reddit.com/r/ArtificialInteligence/comments/1o49454/does_geoffrey_hinton_agree_with_yann_lecun_about/)  
30. Ask HN: Any insider takes on Yann LeCun's push against current architectures?, consulté le janvier 15, 2026, [https://news.ycombinator.com/item?id=43325049](https://news.ycombinator.com/item?id=43325049)  
31. Grounding Multimodal LLMs to Embodied Agents that Ask for Help with Reinforcement Learning \- arXiv, consulté le janvier 15, 2026, [https://arxiv.org/html/2504.00907v5](https://arxiv.org/html/2504.00907v5)  
32. Embodied AI: From LLMs to World Models \- Multimedia and Network Big Data Lab, Tsinghua University, consulté le janvier 15, 2026, [https://mn.cs.tsinghua.edu.cn/xinwang/PDF/papers/2025\_Embodied%20AI%20from%20LLMs%20to%20World%20Models.pdf](https://mn.cs.tsinghua.edu.cn/xinwang/PDF/papers/2025_Embodied%20AI%20from%20LLMs%20to%20World%20Models.pdf)  
33. Why consciousness can't be reduced to code | ScienceDaily, consulté le janvier 15, 2026, [https://www.sciencedaily.com/releases/2025/12/251224032351.htm](https://www.sciencedaily.com/releases/2025/12/251224032351.htm)  
34. Can neuromorphic computing help reduce AI's high energy cost? \- PMC \- NIH, consulté le janvier 15, 2026, [https://pmc.ncbi.nlm.nih.gov/articles/PMC12595464/](https://pmc.ncbi.nlm.nih.gov/articles/PMC12595464/)  
35. Human Brain, AI, Neuromorphic and Quantum: Efficiency, Power, and Profound Design, consulté le janvier 15, 2026, [https://mubbiqureshi.medium.com/human-brain-ai-neuromorphic-and-quantum-efficiency-power-and-profound-design-8a37bbaf99b1](https://mubbiqureshi.medium.com/human-brain-ai-neuromorphic-and-quantum-efficiency-power-and-profound-design-8a37bbaf99b1)  
36. Artificial brains could point the way to ultra-efficient supercomputers \- The Register, consulté le janvier 15, 2026, [https://www.theregister.com/2026/01/09/artificial\_brains\_supercomputer/](https://www.theregister.com/2026/01/09/artificial_brains_supercomputer/)  
37. Neuromorphic Computing Explained: How AI Gets Brain-Like Efficiency \- Rubyroid Labs, consulté le janvier 15, 2026, [https://rubyroidlabs.com/blog/2025/11/future-of-ai-neuromorphic-computing/](https://rubyroidlabs.com/blog/2025/11/future-of-ai-neuromorphic-computing/)  
38. Neuromorphic computing and the future of edge AI \- CIO, consulté le janvier 15, 2026, [https://www.cio.com/article/4052223/neuromorphic-computing-and-the-future-of-edge-ai.html](https://www.cio.com/article/4052223/neuromorphic-computing-and-the-future-of-edge-ai.html)  
39. Does neural computation feel like something? \- Frontiers, consulté le janvier 15, 2026, [https://www.frontiersin.org/journals/neuroscience/articles/10.3389/fnins.2025.1511972/full](https://www.frontiersin.org/journals/neuroscience/articles/10.3389/fnins.2025.1511972/full)  
40. The Functionalist Case for Machine Consciousness: Evidence from Large Language Models, consulté le janvier 15, 2026, [https://www.lesswrong.com/posts/Hz7igWbjS9joYjfDd/the-functionalist-case-for-machine-consciousness-evidence](https://www.lesswrong.com/posts/Hz7igWbjS9joYjfDd/the-functionalist-case-for-machine-consciousness-evidence)  
41. HellaSwag: Understanding the LLM Benchmark for Commonsense Reasoning, consulté le janvier 15, 2026, [https://graphlogic.ai/blog/utilities/hellaswag-understanding-the-llm-benchmark-for-commonsense-reasoning/](https://graphlogic.ai/blog/utilities/hellaswag-understanding-the-llm-benchmark-for-commonsense-reasoning/)  
42. HellaSwag-Pro: A Large-Scale Bilingual Benchmark for Evaluating the Robustness of LLMs in Commonsense Reasoning \- arXiv, consulté le janvier 15, 2026, [https://arxiv.org/html/2502.11393v1](https://arxiv.org/html/2502.11393v1)  
43. What is ARC-AGI? \- ARC Prize, consulté le janvier 15, 2026, [https://arcprize.org/arc-agi](https://arcprize.org/arc-agi)  
44. The Measure of Intelligence (The ARC Benchmark) | by Vishesh Kumar Singh | Medium, consulté le janvier 15, 2026, [https://medium.com/@thevishesh16/the-measure-of-intelligence-the-arc-benchmark-3d85304a920a](https://medium.com/@thevishesh16/the-measure-of-intelligence-the-arc-benchmark-3d85304a920a)  
45. François Chollet thinks arc-agi 6-7 will be the last benchmark to be saturated before real AGI comes out. What are your thoughts? : r/singularity \- Reddit, consulté le janvier 15, 2026, [https://www.reddit.com/r/singularity/comments/1px1g5q/fran%C3%A7ois\_chollet\_thinks\_arcagi\_67\_will\_be\_the/](https://www.reddit.com/r/singularity/comments/1px1g5q/fran%C3%A7ois_chollet_thinks_arcagi_67_will_be_the/)  
46. BIG-Bench Hard | DeepEval by Confident AI \- The LLM Evaluation Framework, consulté le janvier 15, 2026, [https://deepeval.com/docs/benchmarks-big-bench-hard](https://deepeval.com/docs/benchmarks-big-bench-hard)  
47. BIG-Bench Extra Hard \- arXiv, consulté le janvier 15, 2026, [https://arxiv.org/html/2502.19187v1](https://arxiv.org/html/2502.19187v1)  
48. Syntax Without Semantics: Why Generative AI Models Only Appear to Understand \- GitHub, consulté le janvier 15, 2026, [https://raw.githubusercontent.com/AlexHorovitz/academic\_papers/main/ai\_not\_ai/ai\_skepticism.pdf](https://raw.githubusercontent.com/AlexHorovitz/academic_papers/main/ai_not_ai/ai_skepticism.pdf)  
49. Embodied AI: From LLMs to World Models | alphaXiv, consulté le janvier 15, 2026, [https://www.alphaxiv.org/overview/2509.20021v1](https://www.alphaxiv.org/overview/2509.20021v1)  
50. Associative Judgment and Vector Space Semantics \- NSF Public Access Repository, consulté le janvier 15, 2026, [https://par.nsf.gov/servlets/purl/10025982](https://par.nsf.gov/servlets/purl/10025982)  
51. Conceptual Role Semantics | Internet Encyclopedia of Philosophy, consulté le janvier 15, 2026, [https://iep.utm.edu/conceptual-role-semantics/](https://iep.utm.edu/conceptual-role-semantics/)  
52. Computers, meaning, and consciousness | Neuroscience of Consciousness | Oxford Academic, consulté le janvier 15, 2026, [https://academic.oup.com/nc/article/doi/10.1093/nc/niaf057/8377180](https://academic.oup.com/nc/article/doi/10.1093/nc/niaf057/8377180)  
53. A Structured Vector Space Model for Word Meaning in Context \- Stanford NLP Group, consulté le janvier 15, 2026, [https://nlp.stanford.edu/pubs/structuredVS.pdf](https://nlp.stanford.edu/pubs/structuredVS.pdf)

[image1]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAAZCAYAAAA8CX6UAAABD0lEQVR4Xu2SsUoDQRRFrxALixAEwcIqZQqjYKXgB9hYBItA/iJfkG9IUkiaQJo0doqIgrWdZfqQ1g9IEfRe3gzOzG42JKTcAweWeW/vzJtdoGRb7ugXnTubcRm39ImOAi+jDsc5faCP9JdOaSWon9EO/aQrOqAnQT3imL7SG1hYL6oCB3QMCyykAQtSoIJm9DSo+43UV4h26rvnBSys/V/GFf2ABRaiEH/sISzojR65tXCjtYRjCb2sEIUpdKexPBpLQRpTY73QatSRQziWRxetC1dY3kYZdOx3epEWYL+Agp5pKy5lSe8npA4b7Qcb7ueQftMJrSU1zzU2jKWGJezo3m7UYegL3qeLJSX75A/RdzUL5u12HAAAAABJRU5ErkJggg==>

[image2]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAYCAYAAAAcYhYyAAAA00lEQVR4Xu2RIQpCQRCGxyhq8ASCWBTB5CEsXsBjGMxewSiI2OwWo2C0GEWwiGASQez675sdWYc3Lpj3g6+8f97uzA5RIkYPzuAenuEBLuDUO4aNT3WEiVdTgkv4gkOVfVGGGzhQ34U2vMOLDkLq8AqbOvBU4Ja4G5M+cUFVBx7p1DwkWkDc4Y1+1MgorsjCvZU74KEDQUbZ6cBTgHPimrXKMsJRrM2MiPMVLKosIxzF2oxb7RHWdCCEo+RtpgtPZFzQIX4kd0CeT+J3aMkPicQ/vAEKSDOwA0DhWQAAAABJRU5ErkJggg==>

[image3]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA8AAAAaCAYAAABozQZiAAABA0lEQVR4Xu3SMUuCURTG8SPqEAkSQtQQ6CLYUEJEEPQVgginPoCLu6vg19DBPYKGnKXagqaGIFsiWhyCwMGl+t/uVc57Mm5z+cAPeZ/zXricV5E/mwLWkVNdFsvqOZEU9nCBD7xggksU0cHJ9GWdNZzhHedIh979HuEWb9gO/SxVPGGMQ/E30HHPbdxgxcxkhFfs24HKrvhrJ9LEHVbtwMQtr6KLEp7R0OUPcYeXdFEXv9UdXf42PfGHvy0hFvfxB+IP2+1Gk8Gp+MOxuJ205pXucGIRJkX0sWH6r+IBB3YQkhf/Vz22g2nc4BFbpt/EFWoS2clQ/PXv0Q2uUdYvLfK/8gk/KihVrGe+kAAAAABJRU5ErkJggg==>

[image4]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIEAAAAZCAYAAAAWlU1+AAAFgElEQVR4Xu2aaahuUxjH/zJEyHBFMssXmcciIkORDCEZ6n7RjWTKratMvZLig8gQGZNEKCkz5b3UvYYPSqZEuTKEEKGQ4fl59mOvvd79vmfvzjnOeW/rX//O3mutvd+91zM/+0gFBQVTgW2NVxvPMq6fzQU2Ni41nm48WH7N5tXcRsazjdcad6vGCqYIA+PDxnWM2xvfNx6SLqiwu1zwwaPlCsPxGuMzyfGD1TUFiwhYLAJat2X8NeMV1fkWxreMl/23osahyfFmxjurYxRhmVwpUJTv5Io1FvsaXzZ+ZvzQeJFcA1NcKdekuxNyXUF/3GX8wfi38ZvqGJePMhxo3ENuuZdX6zcxDjXZkpHXpcZj8gnDVcZ3jTvlEym2k8eUS+QPxkPtmczzA2jcxcZfjNcYT5DHo4Lu2NL4iPFt48nGDatx3P1K4+Pyvd9B/ZUAxWGePCAFOcHH8nyhE26VuwwU4QPjNo1ZaSu5aynoB6z7W+OfxtOyuQCGRg6AkbHvn2hUCZBPGzDiT40nZuOBuP5z4y7NqSY2NT4t9wDhqi5srJAOk8engn7AFbOf12k0zKYgB3hP7iFI6O6txiOxO686z0EI+EtNJTijGjtXtRL8ZNwnWTMCLPxZ43ryH+ehX2+sGP8QaxsQAhsf7roNJG9LNFmogPlxnjUHSvBAdXy+XB64dwwT5cDlAyw6FThy+dV4UDb2u3xdJJZDuUKMxTmqH4BS5De5JgVQjseS87UV5DkILbi6Of1v8kYy97PxHeNezekRIEDuM8jG23C86vuR6eOZbzC+aLxAtcIhcCw9QNVAGDkgGeN6cgRCyP3yEnNiKEdT0Lp00alyJYjaFJfDw0wbUN6uOFaenKUgISaWM7dcbtFdEW4dK1z0YRQNeknNB0WTCAe3yzWQJOX6ZH6uQD1LSbp3PjFLEAu/V9M6ZgI19nH5oNySsfwfjSdlc5NAIo0bj6bPogbxoy3zJDH8Uu7SnlR7DdoXbEoaG0lUvla/ze0K3qurBRIr8QJtLpMwiSI8p9ESbBK6dupQkJvUroD/C6I0wf3noJzg5R+Vd7AoRWYL3OOkhGuuwHshvK4WiBJQw++aT8i9FF6AsNBHWckvaMLNpATsM+voDywIcFmvqN0CQCRIcyE8rh/kg/OEyIj74DZ5GZzjFnk4IEf6KJubCQPj85rsQeggkm8sCMh0X5XHfr4ytVkN1vGHRjeHjiEZJ6DHsNJ4ptxq8CxodpqhAsIJ3bEAL06uwVqsBos4XF6ZrJA/D9n5C/JuGxiqLnO4f6wjxKRJG9VOXyVAUA8l5+Qr5BbR4OH3CAlvyt+zbb/agAehJX+UmtdQYt6hBey8RhmYlkNYew7WvSH3GIGt5Q2QQXUezYj7jDvK4z5CACgBc6whsQxvwl9CEAoYTSm+RVDuDFULeo2asfIJ1Rk/tXSEKNw4a0GEAtgXKNtXcqFRZ+fVAIpCicZ+5WXZOBwhb91yzRfy7y4oKF3BtNSbKhAXcY/RnIi2JVbNGC8X4YWXpfkU5VIOBEfiGUDIaZLKvcJ74OKjYRWKF5aFl2EtiFAQitgX8XUvvsvnwEPgeSDHXYDXZU/4RnOKcWd19ySLEggb4bFRAEuNcgwhpXUx48ynloorjRiJ0AknUSIiyDRJTXMRBM19WEvoiPsBvAxr6arxHFgyfyfF4oJZAO2/0fiUvL8Qn0EBoWCVXCjU3RHvsGbiOzGQ2AoQEFbPf8+ERQ1VhwKU7MjqGCyTJ2/7V+fkJXzZxL3eLO+wEar2kz/HPdW6gnkEwsr/IQLrpPbHlYYwAwg6d4F4jHRsg+SY8Xx9XqGk/ftQLsC6ce68YJ4xFS3SgvkB1shHDmIx/3SyYGVPQUFBQUFX/AOhDQuOmGQO8AAAAABJRU5ErkJggg==>

[image5]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIEAAAAZCAYAAAAWlU1+AAAFZklEQVR4Xu2aachtUxjH/0KZh0vmuq4hSYYyJYqEyJBMcckHQ4YMpQyZen2QCCFTqNslyRAfREi6uGVMCB8Mea8MIR8oyuz5edZjr3edvffZ5305nffav/r3nr3WOufsvZ71POtZz3mlnp6eecGqpsNNN5i2LfpyNjddZbrHdGHWvrPpDtPRpu3TONQzT1hket+0Z7q+3PSQabV/RlQsV2XcfUyXptenmY5PfehK0ympr2dCWN20qWmdon0t0zGmz01bpbaTTZ/Ix5d8bdohvcbYS9Prs9I17GW6Xv6dtexoutP0qumzpOfl4SV0umm9eEPPnFhsesP0p+kX08+mx+UGx0hnyr15hSojHmn60bR7us5h0QT0T2XXsL7pNtMmRfsMNpbvG3zxH6arTcclnShfWb/Lb6Jn9qxiOkJu+JtNW6c29n6c7APTs6b9NNoiCPisW0wLi/azTecWbY1ca3pM9fsOnGd6xrRm2dHTCt59l9zzibBNsP//JDfmRRpcBN/Jo3YdhPsnTJuVHca0OiaEa8tvMJKKOliFbTfSUw+eyAL40rRd0ZfDdkAeAAeZvjXtmq6xC4kiUbsEz7/dtCBdT1Vdf5Mvpla2MX0lD0VNsAh+VfuYlQE8caMkXtcRSd0aZUcNGJNFQCRtg0XwbnrN/v2W6VD5PWBkQj2vr0h9kTTivGeo2r7z7+H+Xjatm7U1cpT8RutWWoDxyRlYpSszH8vnAhGey+3vEXmOhGezt7eB0fgcPHxR0VeCt2LIgBMCCeQFphdUGf0m06eq9v6419BhqR2I8Ms0eAIZgAHL5B/QBA+zRM0haVLp4qkBxn60po15eVJecOH5SeS6gsPwfo54Ew17PHt9W/a/pTzBICw1hcjZsovpfLWcYWcBC/VF+cLter/svxRkSl6XG5Lt8rmibxic1YkmUfSZWFilPCSrvAn2GsbsVHaMCKHsvqKNayZ3aMgaERbCKB5IBs55umRvuYOwFR5S9A2DhG7Y0Q6Y1/s188w/VjACBsZr6qDY8JJ8TFevaoI9Du8YB0z8sMnPYRFwTC7hme+WP/+okYD9ucsimFL7yew/ZUNV1as6r2ECLpH3UzmcK9Py+vY44Hl4vq6wHdxbNsq9lCoqxhzVEUgGiSBk+U1wxieDj8Rv7Fwsf7C35Uci4CG3kHvs96aTNJgMER1IoqKdTJayMz90ED7JMY6Ve8BHqmoLD6qaRCZoobwmHhkt4yhYfZj6TpBX2PghhPetkHts8E4aBxyNYiJjcY/KwfKMOuAeOYLxvMBzcj+Xaea4Nng/c0xpPi+9M3d834FZ21hh1f+g6lhRiiPQa2p+UAogeEeAYfg8PpfFgwEwBIsAD6Kf63wr2E2ea5CLxJkbg7JoOLIC4TmvUrIIok7BWToPoYyN0wDfm99fV1hoX8jf+43pNw3OwSuq5mlp0VcH7yfXiHkloj4srx8sycbNK+JIiVcHGGNaPom0R4JFSI7FgZeXWTLZeH7iwMAYOiLHU/LoEuRHVBZKfB7GZ2zA984mEkAUglDTiWUD+bmev10hmpBYsvAP0GjH14mDh8dQ4YV4Kd5KgomBMFTkF6z08GTa6Oc1x0IIz6acStmTmnle4aI/ilNMGt7OOMbz/RgKqHgylp9UMQzfi9rKtD1zhFD+pryU+YCqvZhwTyXtaXmla//UDnjudaZzVHn+cvln7JGu30vjAn4UCY8h/N9oukbuoXgWn3erPFqwfZ0q/wGMH2zILf7tY2dPAYlNOclsBUQEjFRXWSzHc52HRfbPWCBQhkyiQN5PMhtj8tDNmPhBpWfM5FtBz/8Q/hmS7Jc6+75FX09PT0/PxPEXD7MITslVhxAAAAAASUVORK5CYII=>

[image6]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAmwAAAAuCAYAAACVmkVrAAAE60lEQVR4Xu3dS4ivYxwH8Eco11xLQue4RsRCEpGSay4LuRXZWJDYUG5ZjGQhFrKgpGQhhSVFxJSF2wLllpKOlCKkUMjl+Xre58w77/nPnGmayTnN51O/5p3nef///8x/9e25vaUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAMA6ObTWk7V2n3YMziztnqtGbZfUerzW0aM2AADWwVytZ4frT2udsdC11Q21Lhv9fmSt04bre2s9N+oDAGCNvVVa6Ir3a90+6usyujZ2Ra3Dh+vran056gMAWOTsWt/V+qfWZ7UOGdp3q/Xw0J56p9ZxQ99Gsktp30u+g+trbap1d62var1e6+VaW2rdNdw/X+uZ4Xrsxlq7loVglvt7iMvI26/DNQDATAkPj5QWSl6Z9L1a66xJ20aR9Wj5TvabdlT71Pq71nmlhbBxYHtsuO72HioS5hLUMgo3Dmw/DNcAADM9X+vi0gLI75O+jKwdNmnbCDKydmet96YdI9/WOqq0UbanhraMtt209Y4mgey24TqB7eDSgt4pQ1vC3ifDNQDATC/U2qPWraWNKGVBfNdHjnY2e5a2a/P+0sLXWKZ2037CpH1svrTvIu+zlAeHnxmBe6nW6bVuKe3zEsh+G/rz+wO1ri0tHHdZ75b73igL69kAAGbqwSNB7ZvSgltk2m9nnQ79qNbXtf4oLSQdOLQnXP1S69Gy/MhhRhsT2FYq69MumDaOHFHr0rI4POZvyWvyWgCAJSW0ZFqvy5EUCStxeWmbD3YkK/l78j+Mz0PL5oCEr/tK20CwPQmquX9+0g4A8L/ICFpfEB+ZAkxYSeCZLp5frbzXydPGVfix1qnTxhn6ERvd5tI2BmS07fzFXTNlM0C+g1m7PbuEOgCAdZfRqvGaqi6jUG+XtuFgNXKu2Hoson+6bLsebZYnpg1lIYRlKnR7EmCXC2wn1Xpz2ggAsB4yHZpDX6ey0SCB5cVpxwplZG49Tu7PIv2VmO7STMi7p7QRtr8mfUtZbko0mxmumTYCAKylBJiDan1Q68Na+y/u/q//z7J4w0Gee5nHLsW+pe14vLC06cdNQ3uOt8hu00w/9scu3VFaAMyoVRbZH1/acRiZJs1i+49rHVPa0Rf9XLLXSjtSI4f4jtecrTSw9YAW+YyfS/s78pk5b+77WlcPfUvJkwgS8PI/dtnJmRC71PNCAQDWTBbl57y1jCKletAae7e088K6BKu54Trrt3LuWEbo8tpuS2mhK9OheW3eM8GnT61uLu28t37a/wFlYUdqRsXye6S/b4bIe0ZCWKZEV+qh0naJZkdoPrNPpeZnf7LD+Nmes5xTFqZGM6r2ea1zF90BALAD6WEsLipt8X/OEOuBKgEr4Suhq09J9qM0MirVNx1kx2bfFJC1bj0U5n0y0paz0fqzOHPcSALhiaV9Xmq5c9EAADa0jHplSjDTmpmyzEhVglefprx56EvgylRqplwTrhLIEsyuHO5LMEvQi4zS9ZGvvM9caWfB5f74orTQltdmNOzYsu1IIAAAI5kKHa/7SvjKdON0DVzC2vi+PtUZe42usxauGx+TkVCW94jxczynnwMAwDJyqO5PZe3OagMAYI3lDLdMZ45HyQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACADeFf3NqxJYOHTPwAAAAASUVORK5CYII=>

[image7]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAmwAAAAuCAYAAACVmkVrAAAExElEQVR4Xu3dS6hvUxwH8CUUeT9KiuRZIuQ5USYGJFIImSgDUkp3QJRyk2Imj0jqZmAgjwkilCsDysAEE+SRRwilGJDH+rb2umfdff/nnnO5h3s7n0/9+u+99v7//+d/Rt/Wa5cCAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABr5MBaj9fab35hclGtI6fXLud31bq21t5DOwAAO9k1td6cjvOa87lba11ea4+h7anp/KhaHw7tAADsZAleqXi21hPDte6s2fkBte6cjg+p9e5wDQBgK1fX+rHWX7W+q/XFVDlPLTfEt568XevPWjfWOrHW9bU+LW0I9INam2s9Od2b15zPbay1b613pvMMh94+He9fFr8HAGCLB0sLZ+NwXRw0td80a18v8v/I78+Q5Vy/lhD3etk6sL3Ub5pkftrh03FCWnrbjpiOQ2ADAFb0VmnhY5G0J5CsR1fU+nreOPi91vmlBd7+P9o8nY8S0B6bjhPSTq61T1kaOk1v2+fTMQDAQgllGdpbJNd+njfuBtIDluCUmq/APKzWDWXx4oAuYSq/PT1hy8l8tb1K+/xHap1Z6/7pPKHsq6Vby8O1rixLQ6LxYq37ar1a6+ahHQBgGwkmfdL8XK59OW/cDTxa2ly8zM/7uNY5U3uC3K+1Xq513tS2yE9l+V7HRfK5F88bBwmJl9bac2jLcYJdhp4BAJaVwJAA0wPNKPOuElo2zS/8jzKUuJIEoBOG89tK+x1ZYPHN0L49ud8wJQCwS7istOHQPil+dGFpqyPHzV7/qVvKtkOTOyp7nCU8zhdHzCV8Zqiyy/fmffktDwzty8kigAS2zbP20WqCIwDAv5a9wLLgICsd506p9X2tc+cXVuG4sja9U5m8P9/PbJFFQ5N9Vef78wvL2F5gy7y2N+aNAABrIcOhP5TFw6FZ9fjHvHGV0jP3ybxxJ7iutE1mV9JXYY4yX63vN7dSD13kvs/mjZM7pgIAWDMJLJkE/1xpweTo0raWSJ1a67daF2y5u8m8sGfK0qT5rHbMTv0JQtn+Ij4qLSxlH7K+i/+xtY4pS71euZ7VlWmLfNdVpX13JuVH5py9VtrfmdWV6QmMHXkawPPD8XulLTKIS0r7zVmdOQ6bzp1dWg9jVpN2eV7oQ8UiAQDgP5DwlNCyqBKgEmrmsnluVl122erj9NKGU3uv1y+lha4Mh6aXLc4obfuMDCOm1ytBLcGue6W0JwAkyGVPs/i2tLl1CVQJd934/SvJb8z9eXrDxtK+o8uTC/Jbs8nt9pxU2n1Pl/ZUg/xdeVA7AMAuKSGs78yf8JN9yrJQoe/flt6wHr7Sw5Zw1ldq5r05PrTWhtLmzUXmuvVgl/fkeu7LcGweiZUAl/eeVtrnbZquAwCwwDjMmSHQ9JRl7lt6sCKLFLJAIcHq3tICXNoiQ5n3lDaUmB6z/iSA9IL1xz4lmGXbjQS4viFterXy3rtrHVxab14PeAAALJD5a9nyostmu72nbdwQNuFqnPQ/vic9Z33S/3hPtt7o7fmsvs3IeE964AAAWKXjS1tF+sL8AgAAu4beo5YeMwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABgXfkbU6y5WlGzuZAAAAAASUVORK5CYII=>

[image8]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAZCAYAAABKM8wfAAACWUlEQVR4Xu2Wv2tUQRDHv8EUBk1EFIRYmUIIBhQsJGBpYSUpLCKWFjb+qNQuXOM/IGIhgqSIiohpTBANGMVCsUkjWIqIViEoKIhEnU/mHffe3Nt9jcoF7gNfDnbezu7OzM6e1GdzM2AaLn43BROmR6Yd0fC3GDfdML0yfSi0ZLpZ0hnTSHtCA1dMrThoHFLH/zvT+ap5g1lV12VOF7tNU/KFfplmTCcLTcudrJu+tSdkIKpElyhH9poumr6bfpvWquaNErpg+ixfi31sq3wRuGp6YBqMhoJzpsemoWgocd10Og6WuGY6K88Am95TsXrwnsmznoWTUAZEOcVh06ryzl6a9sXBEkQfP2SACBOEMkdNz007w3gXY/JUMCEFC/1U/hsinOsOi/LNkMVb8ntTvpxEnyw0ckKeIlKSgo1S48eioYBSOR4HA7fVOdCk3F95zn35XrJsNy3LN5yCRVjsrdKHasWBAJGN5cSGf8g3D0/k+8mCE2oz1wW44e+VTjmHoPZyUFKxNikJAtX2y8VvhFvNJKKXgvbGNweioYC0zsfBAPUZ4dLh95P8IqbKrQLFzyRSXgeX4oX8m7rocoHuyA+VgnlzcVDeUT7Kfd+TZzILKXojn1DXP1nostzOy1MHi1IOucXa/bWOltw/2lo1dXNJ/uGKaVcxxiZH5Sn8Yjpl2lLYInSGh0q3Oubtl2eIek1l6K68ZSY5aPqqzsmieIpfq+FplN/up0r/0aEDlP0uqD6K+GG9fw63Or5WPc2yuntrz0LtNb5KvQTdIf7b6mmOxIE+ff4TfwBtr3fmOrkYrgAAAABJRU5ErkJggg==>

[image9]: <data:image/png;base64,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>

[image10]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA8AAAAbCAYAAACjkdXHAAAA9ElEQVR4Xu2RPw4BQRSHn0QpESEOoCNEoZI4AIVOonAAF5C4BxWRKEkUopE4A6VSo9FpJAqF8PvlzdgxZDnAfsmXnX1/dt7MikQ04PhPWftGCbbgCj7g0bxbO3Bkcn3T88FAtGDqJwwn2PSDJAW3os1dL2dZw5ofJHl4hldYceIFmDHrJSw7uRc8F3fl7pyCJOBC9MNkDrNm/cIdeSd6q3vzznsIxY58gz3RGx7Cu+hEoXwbOQ03EoxMeIwPJqLNfFpycCZBQxzWg3SAPW/YiEWY9IPkYvz6G0R3dad6wz+vSwy24cENVkVvl42/ZB3rIyL+4wm53T9I1ue+FgAAAABJRU5ErkJggg==>

[image11]: <data:image/png;base64,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>

[image12]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAI4AAAAZCAYAAADnnhbzAAADoElEQVR4Xu2YTahNURiGP6HIXyH/EqFkQBkRpVDkr1AMxNDEiEIyQUYmykxKBgaKIkQyUAbKSEqUFFKKJIqS/HzPXee7Z5/v7p+1T/eec3LXU2+39lpr33efd+21vrVFEolEIpH4b1irGuUvJoYF86TN/KeoXqum+4YOM151SvVU9a4hfF1VXWjopGqhDegRzLd5Nt/m2Xz3ImT/RNrM/7DqrWqmb+gwo1XrVHtVL1U3VbsyOqT6qvqrOtEY0wuYbzzjrcg3nunbS5A9nmvlz0PwNt9QfVetaG3uGqtVv1QLfIMEj3jlYXsNPH+QYt94Puobugj5k/0PqZn/NtV91VIJD7W1tblrHJDgZ4xvUDaq/jRUh6rAtvsLbYDnO1Lue71v6CLkT/bvpUb+01SPVWskLFEM3NHSoztQoF2T/BVlkuqBhDbqhlioQa77iw7etrH+Yg3wXbSimG8898pWZfmTPdtUdP6nVedUI1QTpPihOw0FGoVa3opC7YDPs1IvZN72K/6ig/tt8BdrgO+8FWWONH3X8TyUkLnlT/aPJDJ/HoAC1OBGDLycuVbEONVmaS3+qrSqb2QcmMfLLQlvg2mRhGDOqyb29y5nhoSteKdvKOCg6q5qsm+IAN94ZqJkPbPKmO8Y/G9XpalhWDRkz0S2/Mmelyoqfwb52V+2P3cK/jce8EKd47kozUnl/XvYEihUuc8saZ2ERaLfcQnH6T0Sj/nO88wWZr6rPHcCsmfiZL0wYSz/QuaqXkno6PVQQj3QLWar3kg4nXCy8rAH4/Obaplr8+yX0PejtH5fqRL9Gce+H4v5zvMM5rvKcycoyt7yz4VliX2N/c3DwLY+Ag0i1Acs688lfwnme0jsxIFjErYqtqwY2GbY749IvSLWfOd5BvMd43kosdqGv1msPCD/XDhBUUlTUXvsLWPJLoPj2ycZOFvLdLtvZDVnJPRnz/UPB/cktPM3ZtnnHrslLMGcbKqgX2w9lMV853nGp/mO8ex/uyr5YrwM8s/LnmM49xqwyo6UsK+xDC+XgQ/I28X2gDiB+PZOgMcvqp+qlZnreONNxf8L1ZJMWyzzJYRXBist/eqAZwp/850F33aaatf3YIDHxdLM32eLzy3SzL+/HcOfpXWWsnQatox6dYpsQVyk36pnEvfG5sGPcclfdPAxzP+oZeDb+/TC8z5p3/dgUJY9eM9oU0uPYU5V0d/N02QikUgkEolEIpFIJBKJxD+sqhUphQglhAAAAABJRU5ErkJggg==>

[image13]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABsAAAAXCAYAAAD6FjQuAAABaElEQVR4Xu2UQStEURTHz4QihGQhFMWCsmErC6tZUBYWyoKPoCxspCx8AVkoSaxthJ3FlI34ALZ8AAsLNhK/497Je2fmnXlqLNT86lfvnXPf/O+7c+8T+ecUsT+q13Ppdn1Zx0UcxkK6VX+mbcFDZzOKTbYRacExnMJu01NW8RBPcVYy3k6LE3iOjxLW3DKPz3iJRxLGdSUHwA62YS/e4ka6LTKJH/iGn/gk1cPecU1+ZtuHxxLetkxyRXbxIXGfQtf7VaqHae8KW01dJ7cXr3XMQaK3KWElquKFreCJqSk6voQdOIIDsd6MZ3gR7yvwwnSWWWHJ8fu4JGGT6H82GOsVeGG6VHnCdGMs4Lhk7+hvvDANyhOWGy8s7zLmxgvL2iB6XG6w0zZq4YXN4DW2m7pufT1rBVOviRemX4p77DF1DVs2NRf9YX3IWpJwfsps4QtuS1jWOwnf0T9jSMI50rBffeEbNHD5AqK9UIa5/yRhAAAAAElFTkSuQmCC>

[image14]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAAZCAYAAAA8CX6UAAAA8UlEQVR4XmNgGAWkAlsgXgPEs5DwVCBWh8rPRZMD8bECaSAOAeJqIP4LxIeBOBiIuaHy3UD8D4i/AfEMII6AiuMFIEXvgVgHSew0EMsj8YkC4kD8H4gboHwXBjIMgQGQQdeB2A+Ib6HJkQR+MkAMew3EZmhyJIE9DBCD0MOKJMAPxBOB+AYDaliRBFgZINELoicxIMKKJADS3MAAMQgELBkgYQVKP0QDRiAuA+LdDBCvgQAnEO9ggLiKBSqGE4BcMZ0BojiZAWIgDIDYxkD8Foi7gJgDSQ4FeDJADEDGRVA5NiDegEUeFJuwbDMKRgHVAACPkDRrH97rqwAAAABJRU5ErkJggg==>