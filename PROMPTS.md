# Cursor prompt

Tu travailles dans le projet Mos Eisley Cantina.

Respecte strictement les règles définies dans `.cursor/rules/mos-eisley-cantina.mdc`.

Modifie uniquement la section sélectionnée `<section id="features">`.

OBJECTIF

Créer la section Features en HTML sémantique + Tailwind CSS Play CDN en reproduisant le plus fidèlement possible le design de référence fourni.

La section doit être sombre, compacte, centrée et composée d’un titre puis de 3 cartes alignées sur desktop.

CONTRAINTES

- Utilise uniquement HTML + classes Tailwind.
- Ne crée aucun fichier CSS ou JavaScript.
- Ne modifie absolument pas le header ou le hero existant.
- Ne crée aucune nouvelle section.
- Utilise le moins de `<div>` possible.
- Préfère les éléments sémantiques :
  `<section>`, `<header>`, `<article>`, `<h2>`, `<h3>`, `<p>`, `<span>`.
- Chaque carte doit être directement un `<article>`.
- N’utilise aucune librairie d’icônes externe.
- Utilise de petits SVG inline simples pour les icônes.
- Le code doit rester lisible et compréhensible pour un débutant.

SECTION

Conserve :

`id="features"`

et :

`aria-labelledby="features-title"`

La section doit rester centrée avec une largeur proche du reste de la page.

Utilise notamment :

`mx-auto max-w-6xl px-6 py-20`

EN-TÊTE DE LA SECTION

Avant les cartes, crée un petit en-tête centré.

Ajoute exactement ce petit texte au-dessus du titre :

`WHAT YOU FIND INSIDE`

Style souhaité :
- très petit texte
- uppercase
- tracking large
- violet clair
- font-semibold

Ajoute ensuite ce titre principal :

`A booth for every kind of trouble`

Utilise le `<h2 id="features-title">`.

Le titre doit être :
- centré
- blanc / slate très clair
- gras
- taille approximative `text-2xl md:text-3xl`

Sous le titre, ajoute exactement :

`Three things you can count on, any night you walk through the door.`

Le texte doit être :
- petit
- gris clair `text-slate-400`
- centré
- avec un petit espace sous le titre

Garde l’ensemble assez compact, comme sur le modèle.

GRILLE

Sous cet en-tête, crée directement la grille.

Utilise :

`grid grid-cols-1 md:grid-cols-3 gap-6`

Sur mobile :
- 1 carte par ligne

À partir de `md:` :
- 3 cartes sur la même ligne

CARTES

Créer exactement 3 `<article>`.

Chaque `<article>` doit contenir directement :

1. un `<span>` servant de boîte d’icône
2. un `<h3>`
3. un `<p>`

Ne crée PAS de `<div>` supplémentaire dans les cartes.

STYLE COMMUN DES CARTES

Utilise notamment :

`bg-white/[0.03]`
`border border-white/10`
`backdrop-blur`
`rounded-xl`
`p-5`
`transition`
`hover:-translate-y-1`

Les cartes doivent :
- avoir la même hauteur visuelle
- être sombres et légèrement transparentes
- avoir une bordure très discrète
- rester assez compactes
- ressembler au modèle fourni

Les titres doivent être :
- blancs
- `font-semibold`
- environ `text-sm`
- avec un espace sous l’icône

Les paragraphes doivent être :
- `text-sm` ou légèrement plus petit
- `text-slate-400`
- `leading-relaxed`

CARTE 1 — LIVE MUSIC

Icône :
- petit SVG représentant une note de musique
- `aria-hidden="true"`

Boîte d’icône :
`size-12 rounded-xl bg-violet-500/10 ring-1 ring-violet-400/20 text-violet-400`

Titre exact :

`Live music nightly`

Texte exact :

`Sunset to sunrise, loud enough to drown out a bounty hunter.`

CARTE 2 — SMUGGLERS

Icône :
- petit SVG représentant un bouclier
- `aria-hidden="true"`

Même taille et forme que la première boîte, mais avec les couleurs amber :

`size-12 rounded-xl bg-amber-500/10 ring-1 ring-amber-400/20 text-amber-400`

Titre exact :

`Smugglers welcome`

Texte exact :

`No questions asked. Back booths, no records kept.`

CARTE 3 — DROIDS

Icône :
- petit SVG simple ressemblant à un petit droïde / robot ou à l’icône carrée du modèle
- `aria-hidden="true"`

Même taille et forme que les autres, mais avec une couleur violet/fuchsia :

`size-12 rounded-xl bg-fuchsia-500/10 ring-1 ring-fuchsia-400/20 text-fuchsia-400`

Titre exact :

`Droids: see house policy`

Texte exact :

`Limits on the floor. Power-down recommended.`

IMPORTANT POUR LES ICÔNES

Les trois icônes doivent :
- avoir exactement la même taille
- être centrées dans leur boîte
- utiliser `currentColor`
- être simples et discrètes
- avoir des couleurs différentes comme sur le modèle :
  - violet pour la musique
  - amber pour les smugglers
  - fuchsia/violet pour les droids

Ne charge aucune bibliothèque externe.

ACCESSIBILITÉ

- Les SVG décoratifs doivent utiliser `aria-hidden="true"`.
- N’ajoute pas de liens si l’exercice n’en a pas besoin.
- Si tu ajoutes malgré tout un élément interactif, ajoute obligatoirement un état `focus-visible`.
- Conserve une structure HTML valide et sémantique.

RESPONSIVE

À environ 375px :
- les cartes doivent être sur une seule colonne
- aucun débordement horizontal
- les textes restent lisibles
- les espacements restent cohérents

À partir de `md:` :
- exactement 3 colonnes
- cartes de largeur équilibrée

FIDÉLITÉ VISUELLE

Le résultat doit ressembler au maximum à la référence :

- fond sombre violet/noir
- section relativement compacte
- petit label violet centré
- gros titre centré
- petite description centrée
- beaucoup d’espace avant la grille mais sans exagération
- 3 cartes sombres alignées
- cartes légèrement transparentes
- bordure fine
- icônes colorées dans de petits carrés arrondis
- titres blancs
- descriptions gris clair

Évite :
- cartes trop grandes
- gros espaces inutiles
- couleurs trop lumineuses
- ombres importantes
- gros SVG
- wrappers `<div>` inutiles

IMPORTANT

Génère uniquement le code correspondant à la `<section id="features">` sélectionnée.

Ne modifie rien d’autre dans `index.html`.

Avant de terminer, vérifie :
1. qu’il y a exactement 3 `<article>`
2. que la grille utilise `grid-cols-1 md:grid-cols-3 gap-6`
3. que tous les textes demandés sont déjà présents
4. que les 3 icônes ont les bonnes couleurs
5. qu’aucun `<div>` inutile n’a été ajouté
6. que le responsive fonctionne
7. que toutes les classes Tailwind utilisées ont un effet réel
8. que les règles du fichier `.mdc` sont respectées

# Corrections

-J'ai aligner les icones et le texte a gauche (item-start dans head et <<<<<<h3>>>>>>)
- J'ai du reecrire le texte en dessous des titre (simplifié par ia)


# AI Prompts

- Commit 1: Update this Mos Eisley Cantina page using HTML and Tailwind utilities only. Add scroll-smooth to the <html> element, make the navigation sticky at the top of the viewport using sticky, top-0 and z-50, make sure the Menu navigation link points to #menu and the Live Music navigation link points to #live-music, and add the corresponding id attributes if missing. Do not add JavaScript, script tags, event listeners, frameworks, or unrelated changes. 

**Traduction française :**

Mets à jour cette page Mos Eisley Cantina en utilisant uniquement HTML et les classes utilitaires Tailwind.

Pour cette première modification :
- Ajoute `scroll-smooth` à l’élément `<html>`.
- Rends la navigation fixe en haut de la page pendant le défilement avec `sticky`, `top-0` et `z-50`.
- Vérifie que le lien Menu pointe vers `#menu`.
- Vérifie que le lien Live Music pointe vers `#live-music`.
- Ajoute les attributs `id` correspondants aux bonnes sections s’ils sont absents.

N’ajoute pas de JavaScript, de balise `<script>`, d’event listeners, de framework ou de modifications sans rapport avec la demande.

Conserve autant que possible le design et le contenu existants.

- Commit 2: Manual edit — no AI prompt used. Added `shadow-md` to the sticky navigation.
  - Traduction : Modification manuelle — aucun prompt IA utilisé. Ajout de `shadow-md` à la navigation sticky.
