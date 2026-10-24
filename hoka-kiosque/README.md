# HOKA Kiosque — Run Club Paris

Kiosque iPad en caisse : écran de veille, choix de la session, inscription (QR code ou lien).
Un seul fichier autonome (`index.html`), polices embarquées, aucun build.

## Mettre à jour les sessions

- **Sur place, sans toucher au code** : écran des sessions → bouton discret (trois points, en bas à gauche) → code → mode admin.
  Les ajouts sont enregistrés **sur l'iPad** (localStorage), pas dans GitHub.
- **Programme de base** : tableau `RUN_SESSIONS` en haut du `<script>` de `index.html`, puis commit et push.
- **Code admin** : constante `ADMIN_PIN` (à changer avant la mise en ligne).
- **Date du 10 km** (bannière de veille) : constante `KM_DATE`.

## Déploiement (GitHub Pages)

Settings → Pages → Source : *Deploy from a branch* → `main` / `(root)`.
L'URL est `https://<compte>.github.io/hoka-kiosque/`.

## Sur l'iPad

Safari → ouvrir l'URL → Partager → *Sur l'écran d'accueil* (plein écran).
Toujours ouvrir la même URL : les sessions ajoutées en admin sont liées à cette adresse.
Option kiosque : Réglages → Accessibilité → Accès guidé.
