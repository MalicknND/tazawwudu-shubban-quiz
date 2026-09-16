# Le Viatique de la jeunesse — Quiz

**تزود الشبان** (*Tazawwudu-sh-shubbân*)

Un quiz de mémorisation interactif, en une seule page HTML, basé sur le traité versifié
*Le Viatique de la jeunesse* — un texte de théologie, de jurisprudence et de
perfectionnement spirituel (soufisme).

## 🎯 Fonctionnement

- **14 sections** correspondant aux grands thèmes du traité : Préambule, Foi en Dieu,
  les Anges, les Livres Révélés, les Envoyés, le Jour Ultime, le Décret Divin,
  la Purification, les Prières, le Jeûne, l'Aumône Légale, le Pèlerinage,
  le Soufisme, et la Préservation des Membres.
- **Mode par section** : révisez un thème précis.
- **Mode aléatoire** : les questions de toutes les sections sont mélangées.
- Chaque question est accompagnée d'une **explication** et d'une **référence** (numéro
  de vers) tirées exclusivement du texte du traité.
- Écran de résultat avec score, pourcentage et **récapitulatif des erreurs**.
- Thème clair / sombre automatique (basé sur les préférences système).

## 🚀 Utilisation

Aucune installation requise : le quiz est une page HTML autonome (HTML + CSS + JS
dans un seul fichier, sans dépendance externe autre que les polices Google Fonts).

- **En ligne** : voir la section [Démo](#-démo) ci-dessous une fois publié sur GitHub Pages.
- **En local** : ouvrez simplement `index.html` dans votre navigateur.

## 🌐 Démo

Le quiz est accessible en ligne à l'adresse :

**https://malicknnd.github.io/tazawwudu-shubban-quiz/**

## 📖 Source

Toutes les questions et leurs explications sont tirées du traité original :
[`Tazawwudou-sh-subban-fr.pdf`](./Tazawwudou-sh-subban-fr.pdf) (traduction française).

## 🛠️ Enrichir le quiz

Les questions sont définies dans le tableau `SECTIONS` au sein du `<script>` de
`index.html`. Chaque question suit ce format :

```js
{
  q: "Intitulé de la question ?",
  options: ["Option A", "Option B", "Option C", "Option D"],
  correct: 1,           // index (0-3) de la bonne réponse
  explain: "Explication tirée du texte du traité.",
  ref: "Vers X"
}
```

Pour ajouter une question, il suffit d'ajouter un objet à la liste `questions`
de la section concernée (ou de créer une nouvelle section dans `SECTIONS`).

## 📄 Licence

Projet personnel à but éducatif.
