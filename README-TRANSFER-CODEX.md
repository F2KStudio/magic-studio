# Passation Codex - Banner Generator

Derniere mise a jour : 2026-07-30

## Objectif

Ce dossier contient le generateur de banners actuel, avec deux parties :

- `index.html` : outil principal Banner TCG.
- `goods.html` : nouvel outil Goods / Produits.

Les templates HTML exportables sont separes pour pouvoir etre utilises par Make + Doppio.

## Fichiers importants

### Outil principal TCG

- `index.html`
- `desktop-fr.html`
- `desktop-en.html`
- `mobile-fr.html`
- `mobile-en.html`
- `social-fr.html`
- `social-en.html`

### Outil Goods / Produits

- `goods.html` : interface du generateur goods.
- `goods-desktop.html` : rendu web goods.
- `goods-mobile.html` : rendu mobile goods.
- `goods-social.html` : rendu story / insta goods.
- `goods-video.html` : rendu video SNS goods.

## Etat du projet

Le template goods permet :

- 3 visuels/logos a gauche, chacun affichable ou masquable.
- 1 a 5 produits importables.
- Reglages par produit : taille, gauche/droite, haut/bas, calque.
- Lueur autour des produits.
- Formats : web, mobile, story/insta, video.
- Dans `goods.html`, les jauges produits sont deplacees sous l'apercu quand on clique sur previsualiser.

Derniers reglages effectues :

- `goods-video.html` : animation en ligne, sans blocage au milieu.
- La figurine grossit au centre puis redevient plus petite en sortie.
- La ligne video a ete baissee.
- Le passage au centre a ete accelere.
- `goods-desktop.html` : produits agrandis et rapproches.
- `goods-mobile.html` : groupe produits decale vers la gauche.

## Hebergement GitHub Pages

Uploader ces fichiers dans le repo GitHub utilise pour le generateur, par exemple :

`https://github.com/chatgpt-lang/banner-v5`

Si GitHub Pages est active, les URLs publiques devraient ressembler a :

- `https://chatgpt-lang.github.io/banner-v5/index.html`
- `https://chatgpt-lang.github.io/banner-v5/goods.html`
- `https://chatgpt-lang.github.io/banner-v5/goods-video.html`

## Make / Doppio

Pour exporter les nouveaux formats goods, Make doit pointer vers :

- Web goods : `goods-desktop.html`, taille `1562 x 395`
- Mobile goods : `goods-mobile.html`, taille `700 x 420`
- Story / Insta goods : `goods-social.html`, taille `1080 x 1920`
- Video goods : `goods-video.html`, taille `1080 x 1920`

Parametres importants a mapper dans les URLs :

- `left1_url`
- `left2_url`
- `left3_url`
- `show_left1`
- `show_left2`
- `show_left3`
- `figure_count`
- `figure1_url`
- `figure2_url`
- `figure3_url`
- `figure4_url`
- `figure5_url`
- `bg_url`
- `fallback_bg`
- `product_glow`
- `series_text`
- `product1_size`, `product1_x`, `product1_y`, `product1_z`
- `product2_size`, `product2_x`, `product2_y`, `product2_z`
- `product3_size`, `product3_x`, `product3_y`, `product3_z`
- `product4_size`, `product4_x`, `product4_y`, `product4_z`
- `product5_size`, `product5_x`, `product5_y`, `product5_z`

## Reprendre dans Codex sur un nouveau Mac

1. Transferer ce dossier ou le zip `Banner-3.0-experiments.zip`.
2. Ouvrir Codex.
3. Donner a Codex le dossier du projet ou ce README.
4. Dire : "Reprends ce projet a partir du README-TRANSFER-CODEX.md".
5. Ouvrir localement `goods.html` ou `index.html` pour tester.

## Conversation

La conversation Codex complete n'est pas toujours facile a retrouver depuis un autre ordinateur. Ce README sert de passation courte pour reprendre le projet sans devoir relire tout l'historique.

