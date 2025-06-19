# Pourquoi privilégier un LLM local plutôt qu’un service d’IA en ligne ?

## Contexte et sources

Ce document s’appuie sur les orientations établies par le ministère de l’Éducation nationale et de la Jeunesse dans le cadre de la publication suivante :

- **L’IA en éducation – cadre d’usage**, juin 2025  
  [https://www.education.gouv.fr](https://www.education.gouv.fr)  
  (Référence : « l-ia-en-ducation---cadre-d-usage-227697.pdf »)

Il propose une analyse des enjeux liés à l’intelligence artificielle dans le milieu éducatif et met en lumière les avantages concrets de l’exécution locale d’un modèle de langage (LLM), par opposition à l’utilisation de services en ligne.

---

## 1. Un environnement technique favorable à l’autonomie numérique

### Spécifications matérielles

L’exécution d’un modèle d’IA en local repose sur une configuration informatique robuste. L’exemple présenté ci-dessous illustre les caractéristiques idéales pour un usage fluide :

- **Processeur** : Intel Core i7-12700K, 3.60 GHz  
- **Mémoire RAM** : 32 Go (31,8 Go utilisables)  
- **Système d’exploitation** : Windows 64 bits (x64)  
- **Interface tactile** : prise en charge de deux points de contact

Ce type de configuration permet de faire fonctionner efficacement des modèles LLM quantifiés jusqu’à 13 milliards de paramètres, sans recours au cloud.

### Utilisation de la mémoire vive

Les modèles de langage exécutés localement exploitent la mémoire RAM pour plusieurs fonctions essentielles :

- Le **chargement du modèle** en mémoire (4 à 6 Go pour un modèle quantifié 7B, jusqu’à 14 Go pour un modèle 13B)
- La **gestion du contexte conversationnel**
- Le fonctionnement des **bibliothèques d’inférence** (telles que `llama.cpp`)

Cette répartition garantit des performances stables, sans surcharge des ressources locales.

### Outil utilisé : LM Studio

Le logiciel **LM Studio** est ici employé pour faciliter l’utilisation de LLM en local. Il se distingue par :

- Une interface graphique accessible
- Une compatibilité avec les modèles **open source** au format GGUF
- L’absence de connexion Internet pendant l’exécution
- Un accès à des réglages fins pour la génération de texte (température, top-p, etc.)

Ce choix permet une maîtrise complète de l’environnement, tout en restant conforme aux principes de sécurité et de transparence.

---

## 2. Protection des données personnelles

### Cadre réglementaire

Le ministère rappelle que l’utilisation d’IA dans l’éducation doit s’inscrire dans un strict respect du RGPD et des lois françaises sur la vie privée :

> *« Aucune donnée confidentielle ou à caractère personnel ne doit être utilisée avec un service d’IA accessible au grand public. »*  
> — _Cadre d’usage, p. 8_

> *« Il est interdit de demander aux élèves de créer un compte sur ce type de service. »*  
> — _Cadre d’usage, p. 12_

### Avantages de l’exécution locale

L’exécution locale d’un LLM :

- Empêche toute **fuite de données vers des serveurs externes**
- Garantit l’**anonymat total** des échanges
- Évite les risques de **réutilisation ou d’entraînement secondaire** sur des données sensibles

L’utilisateur conserve ainsi le **contrôle total sur ses contenus**, en conformité avec le droit.

---

## 3. Réduction de l’empreinte environnementale

### Une IA sobre, un enjeu éducatif

L’intelligence artificielle générative est une technologie énergivore. Le cadre d’usage insiste sur l’importance de limiter son emploi aux situations réellement justifiées :

> *« Une réponse d’IA générative est en moyenne 10 fois plus énergivore qu’une recherche classique. »*  
> — _Cadre d’usage, p. 6_

> *« Recourir à l’IA doit être justifié par une plus-value pédagogique et évalué à l’aune de son coût écologique. »*  
> — _Cadre d’usage, p. 12_

### Avantages locaux

Le recours à un LLM local :

- Supprime les appels à des centres de données distants
- Permet une **optimisation des modèles** selon les ressources disponibles
- S’intègre dans une **démarche de sobriété numérique** en accord avec l’Éducation au développement durable

---

## 4. Esprit critique et compréhension des technologies

### Objectif pédagogique fondamental

Le ministère insiste sur l’importance de former les élèves à comprendre et questionner les technologies qu’ils utilisent :

> *« L’École doit donner aux élèves les clés pour comprendre cette technologie et développer un esprit critique à son égard. »*  
> — _Cadre d’usage, p. 4_

### Apports de l’utilisation locale

Travailler avec un LLM local, c’est :

- Se confronter à la **structure interne des modèles**
- Comprendre les **limites de l’inférence automatique**
- Développer une posture active face aux outils numériques, loin de la simple consommation passive

Ce positionnement favorise une **autonomie intellectuelle durable**.

---

## 5. Souveraineté technologique

### Critique des solutions externes

Le document officiel identifie clairement les services d’IA en ligne comme problématiques :

> *« Les outils actuellement disponibles sont majoritairement non souverains, non libres, opaques… »*  
> — _Cadre d’usage, p. 4_

### Avantages du LLM local

- L’utilisateur choisit des modèles **libres, auditables et indépendants**
- Il peut **adapter** l’outil à ses besoins, sans contrainte commerciale
- Il évite toute dépendance à un fournisseur externe

Ce choix renforce la **souveraineté numérique individuelle et institutionnelle**.

---

## 6. Respect des principes juridiques et éducatifs

### Alignement avec les exigences officielles

Le cadre rappelle que toute utilisation d’IA dans l’éducation doit respecter les principes de neutralité, de transparence et d’accessibilité :

> *« L’intelligence artificielle ne doit jamais porter atteinte à la relation humaine, ni aux apprentissages. »*  
> — _Cadre d’usage, p. 8_

### Conformité par l’usage local

En exécutant localement un modèle :

- Aucun élève n’est exposé à une technologie non validée
- Le cadre pédagogique est clairement défini
- L’usage reste **transparent, encadré et réversible**

Cela garantit une **intégration respectueuse des principes éducatifs**.

---

## Conclusion

Le choix d’utiliser un **LLM en local**, plutôt qu’un service d’intelligence artificielle en ligne, s’inscrit dans une démarche :

- **Éthique**, par la maîtrise de la donnée
- **Écologique**, par la sobriété numérique
- **Éducative**, par la valorisation de l’esprit critique
- **Juridique**, par le respect du cadre réglementaire
- **Souveraine**, par l’indépendance technologique

Ce modèle d’usage, aligné avec les recommandations ministérielles, montre qu’il est possible de tirer parti de l’intelligence artificielle **de manière consciente, responsable et constructive**.
