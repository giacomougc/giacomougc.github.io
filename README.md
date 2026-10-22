# Giacomo Colomer — Portfolio UGC

Site une page pour Giacomo Colomer, créateur de contenu UGC à Nîmes.
En ligne : https://giacomougc.github.io/

- `index.html` : contenu de la page (+ le JavaScript en bas du fichier)
- `style.css` : mise en forme
- `images/brands/` : logos des marques
- `images/videos/` : miniatures des vidéos, nommées par identifiant YouTube

## Ajouter une vidéo

1. Mettre la vidéo sur YouTube en « Non répertoriée ».
2. Dans `index.html`, copier un bloc `<button class="video" …>` du portfolio et changer :
   - `data-youtube` : l'identifiant (la partie après `watch?v=` ou `/shorts/`)
   - `data-theme` : la thématique (`animaux`, `bien-etre`, `jeux`, `grooming`, `btp`, `bijoux`, `gestion`, `tech`, `mode`)
   - la miniature `images/videos/<identifiant>.jpg` (format vertical 720 × 1280)
   - la durée, la marque (`<b>`) et le titre
3. Optionnel :
   - `data-resultats="*400K* impressions | *33K* clics"` : un badge par résultat, le texte entre `*` passe en gras
   - `data-une="1"` : la vidéo apparaît dans la sélection d'accueil (1 par thématique, le chiffre donne l'ordre)

## Aperçu en local

Les vidéos YouTube ne se lisent pas en ouvrant `index.html` en double-clic (« Erreur 153 ») :
il faut passer par un petit serveur, par exemple `npx serve -l 4340`, puis http://localhost:4340/

## Formulaire de contact

Envoyé par FormSubmit vers giacomo.ugc@gmail.com. Au tout premier envoi depuis le site en ligne,
FormSubmit envoie un e-mail d'activation : cliquer sur le lien pour recevoir les messages suivants.
