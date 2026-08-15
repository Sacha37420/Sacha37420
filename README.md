<h1 align="center">Salut, moi c'est Sacha 👋</h1>

<p align="center">
  Je construis un <strong>lab self-hosted</strong> où onze applications Django&nbsp;+&nbsp;Angular partagent
  une authentification centralisée (Keycloak&nbsp;+&nbsp;LDAP&nbsp;+&nbsp;Caddy),<br>
  et quelques outils de bureau qui tournent en local.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white" alt="Django">
  <img src="https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white" alt="Angular">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Keycloak-4D4D4D?style=flat-square&logo=keycloak&logoColor=white" alt="Keycloak">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/PostGIS-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostGIS">
  <img src="https://img.shields.io/badge/Caddy-1F88C0?style=flat-square&logo=caddy&logoColor=white" alt="Caddy">
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" alt="Playwright">
</p>

---

<table>
<tr>
<td width="50%" valign="top">

<h3>🌐 Applications web — lab SSO</h3>

<p>
Hébergées sur mon serveur, derrière Caddy et Keycloak.<br>
Chaque app est cloisonnée par groupe&nbsp;LDAP : être connecté ne donne accès à rien par défaut.<br>
Infrastructure&nbsp;: <a href="https://github.com/Sacha37420/sso-lab"><strong>sso-lab</strong></a>
</p>

<ul>
<li>
  <a href="https://github.com/Sacha37420/lab-admin"><b>lab-admin</b></a> — portail du lab&nbsp;:
  apps déployées, éditeur de code, gestion des utilisateurs, catalogue de tests E2E.<br>
  <sub>🔒 <code>admins</code></sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/conciergerie"><b>conciergerie</b></a> — gestion locative&nbsp;:
  biens, frais, co-propriétaires, sync des réservations, bilan de capital.<br>
  <sub>🔒 <code>proprietaires</code>, <code>admins</code></sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/carto-lab"><b>carto-lab</b></a> — SIG&nbsp;:
  import de cartes, systèmes de coordonnées, calculs géo, météo France. Instance PostGIS dédiée.<br>
  <sub>🔒 <code>developers</code></sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/atelier-3d"><b>atelier-3d</b></a> — reconstruction 3D
  (COLMAP&nbsp;+&nbsp;OpenMVS, CPU-only), impression 3D, sémantique de bâtiment.<br>
  <sub>🔒 <code>developers</code>, <code>famille</code>, <code>amis</code></sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/robot-lab"><b>robot-lab</b></a> — robots de navigation web
  (Playwright&nbsp;+&nbsp;LLM)&nbsp;: enregistrement de parcours, assistant IA, exécution.<br>
  <sub>🔒 <code>developers</code></sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/restauration"><b>restauration</b></a> — gestion de restaurant&nbsp;:
  fournisseurs, recettes, commandes, paiements, planning, analyses de ventes.<br>
  <sub>🔒 <code>manager</code>, <code>cuisinier</code>, <code>serveur</code></sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/analyse-lora"><b>analyse-lora</b></a> — suivi de capteurs LoRa&nbsp;:
  relevés, mesures, droits par capteur.<br>
  <sub>🔒 <code>developers</code></sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/app-builder"><b>app-builder</b></a> — éditeur visuel de specs
  d'applications&nbsp;: modèles de données, endpoints, pages, pipelines.<br>
  <sub>🔓 tout compte du realm</sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/storage"><b>storage</b></a> — stockage de fichiers du lab&nbsp;:
  espaces personnels, partages par groupe, API consommée par les autres apps.<br>
  <sub>🔒 API interne au lab</sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/arbre-genealogique"><b>arbre-genealogique</b></a> — personnes,
  relations, périodes d'union. Autorisation par arbre (propriétaire / public / partage).<br>
  <sub>🔓 tout compte du realm</sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/traitement-de-fichiers-compils"><b>traitement-de-fichiers-compils</b></a>
  — dépôt de fichiers&nbsp;: édition, suivi des modifications, historique.<br>
  <sub>🔒 <code>developers</code></sub>
</li>
</ul>

</td>
<td width="50%" valign="top">

<h3>💻 Applications à installer sur PC</h3>

<p>
Outils de bureau, à cloner et lancer en local — pas de compte, pas de serveur.
</p>

<ul>
<li>
  <a href="https://github.com/Sacha37420/doc_writter"><b>doc_writter</b></a> — générateur de
  documentations <b>Word</b> et <b>HTML</b> à partir de templates JSON&nbsp;: blocs atomiques
  (titres, tableaux, graphiques matplotlib, logigrammes Word natifs) assemblés en sections
  puis en pages A4. Format documenté pour être pilotable par une IA.<br>
  <sub>🪟 Windows · 🐧 Linux · <code>Python</code> · <code>python-docx</code> · <code>matplotlib</code></sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/picture"><b>picture</b></a> — conversion simple de
  fichiers image, avec scripts de build fournis pour les deux plateformes.<br>
  <sub>🪟 Windows (<code>build.bat</code>) · 🐧 Linux (<code>build.sh</code>) · <code>Python</code> · BSD-3-Clause</sub>
</li>
<li>
  <a href="https://github.com/Sacha37420/reg_vid"><b>reg_vid</b></a> — <!-- ⚠️ description à écrire -->
  une ligne de description à compléter.<br>
  <sub>🪟 Windows · 🐧 Linux · <code>Python</code></sub>
</li>
</ul>

<h4>Installation type</h4>

<pre><code>git clone https://github.com/Sacha37420/picture.git
cd picture
pip install -r requirements.txt
python main.py
</code></pre>

<p>
Pour <b>doc_writter</b>, installation directe depuis le dépôt&nbsp;:
</p>

<pre><code>pip install git+https://github.com/Sacha37420/doc_writter.git
</code></pre>

<p><sub>Chaque dépôt a son propre README avec les prérequis exacts.</sub></p>

</td>
</tr>
</table>

---

### 🧱 Comment le lab est construit

- **Un dépôt parent, onze sous-modules** — chaque application vit dans son propre dépôt GitHub ; `sso-lab` ne référence qu'un commit précis.
- **Scaffold scripté** — `new-app.sh` génère backend, frontend, Docker, ports et client Keycloak ; une nouvelle app hérite automatiquement de l'identité visuelle commune.
- **Double verrou d'accès** — barrière Keycloak côté navigateur *et* vérification `azp` + claim `groups` côté API. Aucun des deux ne suffit seul.
- **Tests de cloisonnement E2E** — un conteneur Playwright partagé vérifie que membre passe, non-membre refusé, même avec une session SSO active.
- **Rotation des secrets à chaud** — clés Django, secrets Keycloak, mots de passe PostgreSQL et LDAP, sans jamais vider un volume.

---

<div align="center">
  <a href="https://github.com/Sacha37420">
    <img src="https://github-readme-stats.vercel.app/api?username=Sacha37420&show_icons=true&hide_border=true&theme=default" alt="Statistiques GitHub de Sacha37420" height="150">
  </a>
</div>
