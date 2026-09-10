# Kora — site vitrine

Création de sites internet sur-mesure et référencement local (SEO)
pour artisans du bâtiment et boutiques indépendantes. Nantes et Loire-Atlantique.

## Contenu

| Fichier | Rôle |
| --- | --- |
| `index.html` | Accueil : constat, avantages, méthode, avis, tarifs, FAQ, CTA |
| `tarifs/index.html` | Formules 690/790/990 € et packs de maintenance 14,90/19,90/29,90 € |
| `blog/index.html` | Article : pourquoi un site change tout pour un artisan |
| `a-propos/index.html` | Présentation, valeurs, comparaison avec une agence |
| `contact/index.html` | Page contact avec formulaire de projet |
| `mentions-legales/index.html` | Mentions légales |
| `favicon-32/192/512.png` | Icônes du site (K Kora sur fond anthracite) |
| `apple-touch-icon.png` | Icône iOS |
| `og-image.png` | Image de partage réseaux sociaux (1200×630) |
| `site.webmanifest` | Manifeste PWA |
| `logo-k.png` | Logo K détouré, fond transparent |
| `robots.txt` | Indexation ouverte + déclaration du sitemap |
| `sitemap.xml` | Plan du site |

Chaque page HTML est **autonome** : polices, styles et scripts sont intégrés.
Aucun build, aucune dépendance, aucun `npm install`.

## Déploiement sur Replit

1. Créez un Repl de type **Static / HTML, CSS, JS**
2. Déposez les fichiers de ce dossier à la racine
3. Lancez : Replit sert `index.html` automatiquement

## Déploiement sur GitHub Pages

1. Poussez les fichiers à la racine de `main`
2. Settings → Pages → Source : `main` / `/ (root)`

## Formulaires

Les deux formulaires (projet et prise de rendez-vous) passent par **Web3Forms**.
La clé d'accès est intégrée dans le HTML ; les demandes arrivent sur
`contact@kora-lab.fr`. Aucun serveur n'est nécessaire.

Le formulaire de rendez-vous envoie en plus deux champs : `creneaux`
(disponibilités cochées) et `format` (Google Meet ou téléphone).

## Google Analytics

Le tag GA4 `G-KNCGG0G9PQ` est présent en tête du `<head>` de chaque page.

## SEO

Chaque page porte son title, sa meta description, ses balises Open Graph et son
canonical. L'accueil embarque des données structurées JSON-LD :
`ProfessionalService` (adresse, téléphone, zones, tarifs, avis) et `FAQPage`.

Le domaine déclaré dans les balises est `https://kora-lab.fr`.
Si vous publiez ailleurs, remplacez cette URL dans les trois fichiers ainsi que
dans `robots.txt` et `sitemap.xml`.

## Reste à faire

- Créer la fiche Google Business Profile (levier n°1 en référencement local)
- Ajouter des photos de réalisations
- Compléter la mention TVA si vous n'êtes pas en franchise en base
