# Réflexion

## TP4

- Comment désigner officiellement le modèle à utiliser ? Avec l'alias `champion` : `models:/churn-model@champion` pointe vers la version choisie, et on peut le déplacer en une ligne sans modifier le code.
- Comment une application peut-elle utiliser le modèle ? Par une requête web à l'API : `POST /predict` avec un JSON, la réponse contient la prédiction.
- Que se passe-t-il quand on change de champion ? On déplace l'alias et on redémarre l'API : le code de l'API et des applications clientes ne change pas.