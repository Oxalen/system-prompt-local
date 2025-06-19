# Pourquoi utiliser un LLM local plutôt qu’un service IA en ligne ?

## Sources

Les informations analysées dans ce document sont issues du cadre officiel suivant :

- **Ministère de l’Éducation nationale et de la Jeunesse**,  
  _L’IA en éducation – cadre d’usage_, juin 2025,  
  [https://www.education.gouv.fr](https://www.education.gouv.fr)  
  (Document consulté : « l-ia-en-ducation---cadre-d-usage-227697.pdf »)

---

## Spécificités techniques et configuration

### Matériel utilisé

L’environnement local repose sur un appareil aux caractéristiques suivantes :

- **Processeur** : 12th Gen Intel(R) Core(TM) i7-12700K @ 3.60 GHz  
  (16 cœurs hybrides, excellente gestion multitâche et performances élevées)
- **Mémoire vive (RAM)** : 32 Go (31,8 Go utilisables)  
  (suffisante pour exécuter localement des modèles LLM quantifiés)
- **Système** : Windows 64 bits, architecture x64
- **Écran tactile** : Prise en charge du tactile (2 points de contact)

Ces spécifications permettent de faire tourner efficacement des modèles LLM locaux jusqu’à **7B ou 13B de paramètres**, en mode quantifié (GGUF 4-bit, 5-bit ou 8-bit) sans saturation de la mémoire.

---

### Utilisation de la mémoire vive par un LLM local

Lorsqu’un **Large Language Model** est exécuté en local, la mémoire vive est utilisée pour :

- **Charger le modèle dans la RAM** : par exemple, un modèle quantifié 7B 4-bit prend environ **4 à 6 Go de RAM**. Un modèle 13B peut atteindre **12 à 14 Go**.
- **Maintenir le contexte des requêtes** : plus le contexte est long (nombre de tokens conservés), plus la mémoire est sollicitée.
- **Stocker les bibliothèques du moteur d’inférence** (ex. llama.cpp) et gérer le processus de génération.

L’utilisation d’un LLM en local demande donc une machine suffisamment équipée, surtout en RAM, pour garantir la fluidité des échanges sans ralentissement.

---

### Logiciel utilisé : LM Studio

Pour exécuter les modèles localement, le logiciel **LM Studio** est utilisé. Il offre :

- Une interface graphique conviviale compatible avec **llama.cpp**
- La possibilité d’importer des modèles **GGUF quantifiés**
- Un accès rapide et hors-ligne à des modèles open source (ex. Mistral, LLaMA, Nous, Phi, etc.)
- Le support des paramètres de génération (température, top-p, fréquence, longueur maximale)
- Une exécution en **inférence locale**, sans appel à Internet ni cloud

Ce logiciel est particulièrement adapté à une utilisation responsable, éthique et autonome de l’IA.

---

## 1. Respect de la vie privée et des données personnelles

### Interprétation du document

Le cadre d’usage précise que les IA accessibles au grand public ne doivent **jamais être utilisées pour traiter des données personnelles ou confidentielles**. Il est également interdit de demander à des élèves de créer des comptes sur ces services.

> *« Le recours aux services d’IA accessibles au grand public est autorisé sous réserve qu’aucune donnée confidentielle ou à caractère personnel ne soit utilisée. »*  
> *– page 8*

> *« Ne demandez en aucun cas aux élèves de se créer un compte personnel auprès de services d’IA accessibles au grand public. »*  
> *– page 12*

### Avantage du LLM local

Un LLM local ne transmet **aucune donnée à des serveurs distants**. Il permet :

- La protection intégrale des données utilisées
- L'absence de risque lié à la réutilisation ou au stockage externe
- Un traitement local et sécurisé

---

## 2. Réduction de l’impact environnemental

### Interprétation du document

Les IA génératives sont très gourmandes en ressources. Le cadre d’usage appelle à une utilisation **frugale**, en particulier dans l’éducation, dans le cadre de la stratégie nationale bas-carbone.

> *« La production d’une réponse textuelle à un prompt est en moyenne 10 fois plus énergivore qu’une requête sur un moteur de recherche. »*  
> *– page 6*

> *« Renoncez à l’IA si une autre solution moins coûteuse écologiquement peut répondre à votre besoin. »*  
> *– page 12*

### Avantage du LLM local

Un LLM local :

- Peut être exécuté sur des machines adaptées, avec une consommation maîtrisée
- Évite les allers-retours réseau et les charges liées aux serveurs distants
- Permet une optimisation du modèle en fonction des ressources disponibles

---

## 3. Esprit critique et autonomie numérique

### Interprétation du document

L’un des objectifs pédagogiques essentiels est d’amener les usagers (élèves, enseignants) à **comprendre les technologies utilisées**, à en mesurer les enjeux et à les manipuler de façon critique.

> *« L’École doit donner aux élèves les clés pour comprendre cette technologie… et développer un esprit critique à son égard. »*  
> *– page 4*

> *« L’usage et l’enseignement de l’IA doivent être éclairés… »*  
> *– page 10*

### Avantage du LLM local

En installant et utilisant toi-même un modèle local, tu :

- Développes une compréhension plus fine des mécanismes de l’IA
- Ne dépends pas d’une interface préconstruite ou opaque
- Te formes à la fois à la pratique et à l’analyse critique des IA

---

## 4. Souveraineté et contrôle des outils

### Interprétation du document

Les IA « grand public » sont souvent décrites comme :

> *« non souveraines, non libres, opaques dans leur fonctionnement et leurs données d’entraînement. »*  
> *– page 4*

### Avantage du LLM local

Utiliser un LLM local permet de :

- Choisir un outil libre ou open source, dont le fonctionnement est documenté
- S’affranchir des plateformes propriétaires américaines ou chinoises
- Contrôler le cycle complet du traitement : données, modèle, réponses

---

## 5. Conformité au cadre juridique et éducatif

### Interprétation du document

Le cadre impose de **n’utiliser que des solutions qui respectent la législation** (RGPD, droit d’auteur, protection des mineurs, etc.). Or, les services IA en ligne ne garantissent pas ce respect.

> *« Le cadre d’usage précise que l’IA ne doit pas porter atteinte [...] aux apprentissages des élèves, ni aux pratiques professionnelles des personnels. »*  
> *– page 8*

> *« L’utilisation des solutions libres doit être privilégiée. »*  
> *– page 8*

### Avantage du LLM local

En travaillant localement :

- Tu respectes le RGPD sans dépendre d’un tiers
- Tu choisis les données d'entraînement ou tu vérifies leur origine
- Tu restes en conformité avec les principes déontologiques du service public

---

## Conclusion

Tu as préféré utiliser un LLM local plutôt qu’un service web d’IA, car cette décision :

- Protège les données personnelles
- Réduit ton impact environnemental
- Encourage une meilleure compréhension de la technologie
- Préserve la souveraineté numérique
- Respecte le cadre éthique et légal défini par le ministère de l’Éducation nationale

Cette démarche n’est pas seulement technique : elle est aussi **citoyenne, responsable et éducative**.
