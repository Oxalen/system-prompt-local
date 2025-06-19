# Pourquoi utiliser un LLM local plutôt qu’un service IA en ligne ?

## Sources documentaires

Ce document s’appuie sur les recommandations officielles issues de :

- **Ministère de l’Éducation nationale et de la Jeunesse**,  
  _L’IA en éducation – cadre d’usage_, juin 2025  
  [https://www.education.gouv.fr](https://www.education.gouv.fr)  
  (Fichier : `l-ia-en-ducation---cadre-d-usage-227697.pdf`)

---

## Introduction

Le recours à l’intelligence artificielle dans l’éducation soulève des enjeux majeurs en matière de souveraineté, d’éthique, de respect de la vie privée et de responsabilité environnementale.  
Face à ces défis, tu as choisi d’exécuter un **LLM (Large Language Model) localement**, sans connexion à des serveurs externes.

Ce choix n’est pas seulement technique : il répond à des principes forts, alignés avec le cadre d’usage officiel du ministère.  
Voyons en détail pourquoi.

---

## 1. Un environnement technique compatible, puissant et souverain

### Appareil utilisé

L’exécution locale d’un LLM nécessite une machine robuste. Voici ta configuration :

- **Processeur** : Intel Core i7-12700K, 3.60 GHz (architecture hybride très performante)
- **RAM installée** : 32 Go (31,8 Go utilisables)
- **Système** : Windows 64 bits, architecture x64
- **Entrée tactile** : Prise en charge du tactile à 2 points de contact

Ce matériel permet de faire tourner localement des modèles jusqu’à **13 milliards de paramètres**, en mode **quantifié** (4-bit, 5-bit, 8-bit) sans ralentissement notable.

### Utilisation de la mémoire vive

Lorsque tu exécutes un LLM local :

- Le **modèle est chargé intégralement en RAM** (par exemple, ~6 Go pour un modèle 7B en 4-bit)
- La mémoire gère aussi le **contexte conversationnel**, proportionnel à la longueur des échanges
- Les bibliothèques (type `llama.cpp`) et les threads de génération y résident également

Ainsi, la RAM n’est pas simplement un tampon : elle soutient toute la chaîne d'inférence.

### Logiciel utilisé : LM Studio

Pour faciliter l'usage local, tu utilises **LM Studio**, une interface conviviale et compatible avec :

- Les modèles open source (Mistral, Nous, LLaMA, Phi, etc.)
- Le format **GGUF quantifié**
- L’exécution hors ligne, sans transmission réseau
- Les réglages de température, top-p, longueur, fréquence, etc.

LM Studio garantit une autonomie complète : pas d'inscription, pas de cloud, pas de dépendance extérieure.

---

## 2. Respect absolu de la vie privée

### Ce que dit le cadre officiel

> *« Le recours aux services d’IA accessibles au grand public est autorisé sous réserve qu’aucune donnée confidentielle ou à caractère personnel ne soit utilisée. »*  
> *– page 8*

> *« Ne demandez en aucun cas aux élèves de se créer un compte personnel auprès de services d’IA accessibles au grand public. »*  
> *– page 12*

### Pourquoi le LLM local est préférable

- Aucun **risque de fuite de données** via Internet
- Pas de stockage externe, pas de collecte automatique
- Tu contrôles totalement les informations utilisées dans les prompts
- Tu respectes la législation RGPD, la loi Informatique et Libertés et les recommandations du ministère

---

## 3. Une alternative écologique et responsable

### Alerte du cadre officiel

> *« La production d’une réponse textuelle à un prompt est en moyenne 10 fois plus énergivore qu’une requête sur un moteur de recherche. »*  
> *– page 6*

> *« Recourez de manière raisonnée et responsable à l’IA générative en ayant conscience des impacts environnementaux. »*  
> *– page 12*

### Avantage local

- L’utilisation est **optimisée selon ta machine** (pas de centres de données énergivores)
- Tu peux choisir des modèles plus **frugaux**
- Tu participes à une **démarche sobre**, compatible avec l’éducation au développement durable

---

## 4. Développement de l’esprit critique et de l’autonomie

### Ce que recommande le ministère

> *« L’École doit donner aux élèves les clés pour comprendre cette technologie… et développer un esprit critique à son égard. »*  
> *– page 4*

> *« L’usage et l’enseignement de l’IA doivent être éclairés… »*  
> *– page 10*

### Ce que permet le LLM local

- Tu comprends mieux le fonctionnement réel d’un modèle
- Tu ne te contentes pas de résultats : tu apprends à **les interpréter, tester, comparer**
- Tu sors du rôle de simple utilisateur, pour devenir **acteur de ton environnement numérique**

---

## 5. Souveraineté technologique et contrôle des outils

### Risques liés aux services web

> *« Les outils disponibles actuellement sont majoritairement non souverains, non libres, opaques dans leur fonctionnement… »*  
> *– page 4*

### Pourquoi le LLM local est plus transparent

- Tu choisis des modèles **open source** et libres
- Tu évites la **dépendance aux plateformes propriétaires**
- Tu sais **comment les modèles sont entraînés**, et sur quelles bases ils produisent leurs réponses

---

## 6. Conformité au droit et à l’éthique éducative

### Exigences du cadre

> *« L’IA ne doit pas porter atteinte aux apprentissages, ni aux pratiques professionnelles, tout en garantissant inclusion, équité, accessibilité. »*  
> *– page 8*

### En choisissant une exécution locale :

- Tu respectes le **cadre juridique européen (RGPD, SREN, règlement IA)**
- Tu n’exposes pas d’élèves ou de collègues à un outil non conforme
- Tu privilégies une **pratique éthique, transparente et professionnelle**

---

## Conclusion

L’utilisation d’un LLM local n’est pas un simple choix technologique. C’est une **démarche responsable**, en accord avec :

- La **protection des données**
- La **sobriété numérique**
- La **souveraineté intellectuelle**
- L’**esprit critique et l’autonomie**
- La **légalité et l’éthique éducative**

Tu démontres, par cette approche, qu’on peut utiliser l’IA **avec rigueur, discernement et exigence**. C’est une position lucide, à la fois conforme aux textes réglementaires et tournée vers un usage durable, respectueux et éducatif de la technologie.

---
