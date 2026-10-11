# Portfolio — HERIMALALA MANOANIAVO

Site statique (HTML/CSS/JS, sans dépendance) en deux langues :

- `index.html` : version française → https://hery5993.github.io/herimalala/
- `en/index.html` : version anglaise → https://hery5993.github.io/herimalala/en/

## Publier sur GitHub Pages

1. Créer sur GitHub un dépôt nommé **herimalala** (compte `hery5993`).
2. Depuis ce dossier :

   ```bash
   git init
   git add .
   git commit -m "Portfolio"
   git branch -M main
   git remote add origin https://github.com/hery5993/herimalala.git
   git push -u origin main
   ```

3. Sur GitHub : **Settings → Pages → Build and deployment → Deploy from a branch**, branche `main`, dossier `/ (root)`.
4. Après une à deux minutes, le site est en ligne à l'adresse ci-dessus.

Si le nom du dépôt ou du compte est différent, remplacer `https://hery5993.github.io/herimalala/` dans `index.html`, `en/index.html`, `sitemap.xml` et `robots.txt`.

## Référencement (SEO)

- Balises `title`, `description`, `canonical`, Open Graph et Twitter Card pour chaque langue.
- `hreflang` fr / en / x-default entre les deux pages.
- Données structurées schema.org (Person, WebSite, ProfilePage) en JSON-LD.
- `sitemap.xml` et `robots.txt`.
- À faire après la mise en ligne : ajouter le site dans [Google Search Console](https://search.google.com/search-console) et soumettre `sitemap.xml`.
- Vérifier l'aperçu de partage avec le débogueur de partage de Facebook ou l'aperçu d'URL LinkedIn.

## Personnaliser

- **Projets** : modifier les cartes `.proj` dans les deux fichiers HTML. Pour une vraie capture, remplacer le `src` de l'image (format 16/9). Pour un lien dépôt/démo, ajouter dans `.proj-body` : `<a class="open" href="https://…" target="_blank" rel="noopener noreferrer">Voir le projet</a>`.
- **Expérience** : les zones en pointillés sont modifiables dans le navigateur mais ne sont pas enregistrées pour les autres visiteurs. Pour les rendre définitives, remplacer chaque `<div class="ed" …></div>` par du texte ou une liste `<ul>`.
- **Images** : `assets/` contient des illustrations originales (aucune licence à citer) et l'image de partage `og-image-fr.png` / `og-image-en.png` (1200×630).
