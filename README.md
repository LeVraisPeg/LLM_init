# LLM_init

Un projet d'initiation au LLM avec des exercices pratiques pour comprendre et manipuler des modèles de langage.

##  Description

Ce repository contient deux notebooks Jupyter qui vous guideront à travers les bases de l'IA générative en manipulant et en contrôlant un LLM installé en local.

## Contenu

### 1. Copie_de_TP_initiation_llm.ipynb
Notebook principal qui couvre :
- Installation des dépendances (transformers, torch)
- Chargement du modèle FLAN-T5
- Tokenisation et décodage de texte
- Interrogation basique du LLM
- Résumé de dialogues avec le dataset DialogSum
- Techniques de prompt engineering (zero-shot, one-shot, few-shot)

### 2. MyLLM.ipynb
# Mini-projet — Système de Questions-Réponses avec Évaluation Automatique

## Objectif
L’objectif de ce mini-projet est de concevoir un système de questions-réponses basé sur un modèle de langage (LLM) appliqué à un domaine spécifique (le cinéma), et d’évaluer automatiquement la qualité des réponses générées selon différentes stratégies de prompting.

---

## Description du projet
Le projet s’articule autour de trois axes principaux :

1. **Création d’un dataset**
   - Élaboration d’un jeu de données de 15 questions-réponses portant sur des notions fondamentales du cinéma.
   - Chaque question est associée à une réponse de référence servant de base pour l’évaluation.

2. **Génération de réponses avec un LLM**
   - Utilisation du modèle **Qwen2.5-3B-Instruct** via la bibliothèque Transformers.
   - Comparaison de trois approches de prompting :
     - **Zero-shot** : aucune démonstration fournie
     - **One-shot** : une paire question-réponse en exemple
     - **Few-shot** : plusieurs paires question-réponse en exemple
   - Test de différentes configurations de génération (température, top_p, top_k).

3. **Évaluation automatique de la qualité**
   - Calcul d’un score combinant :
     - la similarité sémantique entre la réponse générée et la réponse de référence (embeddings),
     - une contrainte sur la longueur de la réponse.
   - Comparaison des performances des approches en termes de qualité moyenne et de robustesse.

---

## Méthodologie
- Domaine : cinéma  
- Nombre de questions : 15  
- Modèle de langage : Qwen2.5-3B-Instruct  
- Approches testées : zero-shot, one-shot, few-shot  
- Évaluation : score automatique (similarité sémantique + ratio de longueur)

---

## Technologies utilisées
- Python
- Transformers (Hugging Face)
- Sentence-Transformers
- PyTorch
- Matplotlib


