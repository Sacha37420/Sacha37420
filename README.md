# Salut, moi c'est Sacha 👋

Je construis et j'exploite **sso-lab**, un lab self-hosted qui héberge plusieurs applications
web derrière une authentification centralisée (Keycloak + LDAP + Caddy).

## 🧩 Le lab

| Repo | Description |
|---|---|
| [sso-lab](https://github.com/Sacha37420/sso-lab) | Infra du lab — Keycloak, LDAP, Caddy, orchestration des apps en sous-modules |
| [lab-admin](https://github.com/Sacha37420/lab-admin) | Console d'administration du lab |
| [carto-lab](https://github.com/Sacha37420/carto-lab) | Plateforme SIG web — GeoDjango/PostGIS + Angular/OpenLayers |
| [app-builder](https://github.com/Sacha37420/app-builder) | Designer visuel fullstack avec assistant IA |
| [analyse-lora](https://github.com/Sacha37420/analyse-lora) | Gestion et visualisation de capteurs LoRa |
| [restauration](https://github.com/Sacha37420/restauration) | Gestion de restaurant (caisse, stock, paiements) |
| [arbre-genealogique](https://github.com/Sacha37420/arbre-genealogique) | Arbre généalogique interactif |
| [traitement-de-fichiers-compils](https://github.com/Sacha37420/traitement-de-fichiers-compils) | Atelier de traitement de fichiers dans le navigateur |

Chaque application est un sous-module Django + Angular indépendant, cloisonné par groupe LDAP
derrière le même realm Keycloak.

## 🛠️ Stack

Django · Angular · Keycloak · PostgreSQL/PostGIS · Docker Compose · Caddy
