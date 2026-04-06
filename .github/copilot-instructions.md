---
applyTo: "**"
---

# HLTherapies - Site web statique

## Projet
Site vitrine HTML/CSS statique pour Helene Lardeur, psychopraticienne, sophrologue et NAPSOtherapeute a Aix-en-Provence et La Ciotat. Heberge sur GitHub Pages.

## Stack technique
- HTML5 semantique pur (pas de framework)
- CSS custom avec variables (pas de framework CSS)
- JavaScript vanilla minimal (menu mobile, phone reveal, dropdown nav)
- Icones : SVG inline (Lucide-style) -- pas de icon font externe
- Hebergement : GitHub Pages (organisation hltherapies)
- Repo : https://github.com/hltherapies/hltherapies.github.io
- Domaine : www.hltherapies.com (DNS chez viaduc.fr)
- URL temporaire : https://hltherapies.github.io

## Structure
```
/                        -> index.html (accueil)
/helene-lardeur-.../     -> page therapeute
/psychotherapie-individuelle-.../ -> page psycho individuelle
/psychotherapie-de-couple-.../    -> page couple
/sophrologie-.../                 -> page sophrologie
/napsotherapie-.../               -> page napsotherapie
/informations-pratiques-.../      -> page tarifs/infos
/prendre-rendez-vous-.../        -> page contact
/blog/                   -> page blog (vide)
/mentions-legales/       -> mentions legales
/plan-du-site/           -> plan du site
/404.html                -> page erreur
/assets/css/style.css    -> feuille de styles unique
/assets/images/          -> images du site
/assets/docs/            -> PDFs deontologie
/sitemap.xml             -> sitemap SEO
/robots.txt              -> robots SEO
/CNAME                   -> domaine custom GitHub Pages
```

## Conventions

### HTML
- Chaque page est un dossier avec un index.html (URLs propres sans .html)
- Toutes les pages partagent le meme header, nav et footer
- Navigation avec dropdown "Pratiques" (4 sous-pages)
- Liens internes en absolu depuis la racine : `/napsotherapie-a-aix-en-provence/`
- Assets en relatif depuis les sous-dossiers : `../assets/css/style.css`

### CSS
- Variables CSS dans :root (couleurs, polices, espacements)
- Palette : #87786C (texte), #D4B89E (accent caramel), #F2CCC7 (rose), #999494 (gris)
- Polices : Playfair Display (titres), Parisienne (decoratif), Lucida Sans (corps)
- Mobile-first, breakpoints a 768px et 1024px

### SEO
- Chaque page a : title, meta description, canonical, Open Graph, Schema.org JSON-LD
- Les URLs doivent rester identiques a celles de l'ancien site Simplebo (pour ne pas perdre le referencement)
- sitemap.xml et robots.txt a la racine

### Contenu
- Tout le texte est en francais avec les accents corrects
- Le contenu appartient a Helene Lardeur, ne pas le modifier sans validation
- Les photos sont creditees a tiphainetbn.photography
- La prise de RDV passe par Resalib (lien externe)

### Ne pas faire
- Ne pas ajouter de cookies ou de tracking (c'est un choix delibere)
- Ne pas ajouter de JavaScript framework
- Ne pas modifier les URLs des pages (impact SEO)
- Ne pas supprimer les fichiers CNAME, sitemap.xml, robots.txt
- Ne pas utiliser d'emojis dans le code ou les commentaires
