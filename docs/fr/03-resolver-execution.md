# 3. Resolver et exécution

Le resolver indique si une tâche est prête. Il peut lire l’état d’un protocole externe, mais l’exécution finale doit encore respecter les garde-fous du contrat Automate.

Le worker transmet les données et l’appel à la cible. Le contrat vérifie que le resolver et le créateur correspondent à la tâche enregistrée, puis applique les limites de gas et de paiement.

Les callbacks et les retours de la cible sont des frontières de confiance. Le code doit éviter qu’un échec partiel consomme un budget sans fournir l’état attendu.

Une tâche idempotente reste préférable : un même déclenchement ou une reconnexion ne devrait pas produire deux effets économiques incompatibles.

Suite : [permissions et limites](04-permissions-limites.md).
