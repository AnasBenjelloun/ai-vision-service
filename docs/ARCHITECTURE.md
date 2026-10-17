
# AI Vision Service - Architecture

## 1. Objectif

Construire un microservice autonome d'intelligence artificielle avec Java et Spring Boot.

Premier cas d'utilisation : analyse visuelle de graphiques financiers pour détecter des figures chartistes.

Le service doit rester réutilisable par d'autres applications.

## 2. Responsabilités

### AI Vision Service
- Intégration des modèles IA multimodaux
- Analyse visuelle d'images
- Identification de figures chartistes potentielles
- Production de réponses structurées
- Gestion et versionnement des prompts
- Évaluation de la qualité des analyses
- Observabilité et maîtrise des coûts IA

### MarketPulse
- Acquisition des données OHLCV
- Scanner multi-cryptomonnaies
- Génération des graphiques
- Indicateurs techniques
- Validation des opportunités de trading
- Backtesting et gestion du risque
- Présentation des résultats

MarketPulse consomme AI Vision Service via une API REST.

AI Vision Service ne prend aucune décision d'achat ou de vente.

## 3. Stack technique envisagée

- Java
- Spring Boot
- Spring AI
- API REST / JSON
- Modèle multimodal à sélectionner

Les autres technologies seront introduites progressivement pendant la formation.

## 4. Principes d'architecture

- Séparation des responsabilités
- API versionnée
- Faible couplage entre les applications
- Gestion explicite des erreurs et timeouts
- Tests automatisés
- Architecture évolutive
- Aucune base de données partagée
- Sécurité des secrets et clés API

## 5. Architecture initiale

MarketPulse
    |
    | REST / HTTP
    v
AI Vision Service
    |
    | Spring AI
    v
Modèle IA multimodal

## 6. État

Architecture initiale proposée.
Aucune implémentation validée.

Les décisions techniques définitives seront documentées au fur et à mesure de la formation.
