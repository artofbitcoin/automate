# 1. Vue d’ensemble de Gelato Automate

Gelato Automate permet de déclencher des appels de contrats selon une logique de tâche. Le dépôt actuel s’appuie sur Gelato Functions et conserve les contrats qui enregistrent et exécutent ces tâches.

Le système sépare le créateur de tâche, le resolver, le worker et la cible appelée. Cette séparation rend explicite la frontière entre condition vérifiée et transaction effectivement envoyée.

Une tâche peut être financée, exécutée puis arrêtée. Les contrats vérifient les paramètres, les autorisations et les dépenses avant de transmettre l’appel.

Ce parcours décrit le code et les limites du modèle d’automatisation, sans installer, compiler ou déployer le projet.

Suite : [création et financement d’une tâche](02-taches-financement.md).
