# Notes de travail — points en suspens et décisions

*Depuis le message du 30 mai 2026 sur la figure TikZ et les cas limites*

---

## 1. Figure TikZ de la Section I — à améliorer

**Problème :** La première version de la figure TikZ (arbre + organigramme) était peu lisible : nœuds trop petits, espacement insuffisant, Agent 3 en position ambiguë.

**État actuel :** Une version améliorée a été produite (symétrique, 4 enfants pour l'arbre, organigramme à 2 départements sans Agent 3). Visible dans `Sections/01_probleme.tex`.

**À faire :** Compiler dans Overleaf et vérifier la lisibilité réelle sur PDF. Si encore insuffisant, options : augmenter les `level distance` et `sibling distance`, ou passer à une figure externe dessinée manuellement.

---

## 2. Carte bibliométrique — figure externe

**Source :** Figure 5 de l'article *Bibliometric Analysis of Sports Running Socks Made from Bamboo, Cotton, and Acrylic* (Mora-Muñoz et al., 2025). DOI : `10.56294/dm2025831`. Licence **CC-BY 4.0** — utilisable avec attribution.

**Fichier :** `figures/bibliometric_map.png` (à uploader dans Overleaf dans un dossier `figures/`).

**Référence BibTeX :** `moraMunoz2025` — déjà dans `bibliography.bib`.

**Usage dans le texte :** Section I, premier paragraphe, pour illustrer ce qu'est une carte bibliométrique. La légende explique que les couleurs indiquent des communautés thématiques et que la proximité encode la similarité sémantique.

---

## 3. Arbre de Babenberg — cas limite pour la Section VI

**Source :** Wikimedia Commons, catégorie *Babenberg Family Tree* (domaine public). URL : `https://commons.wikimedia.org/wiki/Category:Babenberg_Family_Tree`

**Pourquoi c'est important :** C'est un contre-exemple difficile pour la thèse. C'est indéniablement un arbre généalogique, mais il possède une structure spatiale riche, raconte une histoire, et invite l'exploration visuelle non-linéaire. Il met le critère de métrique globale sous tension.

**Ce qu'il teste :** La richesse spatiale et narrative d'une représentation peut-elle lui conférer des propriétés cartographiques ? Deux figures non adjacentes dans l'arbre de Babenberg ont-elles une relation implicite dérivable de leur position — ou faut-il quand même suivre les liens généalogiques ?

**Position dans le texte :** Section VI (tests), avec ce cadrage explicite :
> *"Tous les arbres ne sont pas également éloignés de la carte. Certaines représentations généalogiques acquièrent progressivement des propriétés cartographiques."*

**À faire :** Choisir une image dans la catégorie Wikimedia (vérifier la licence — la plupart sont domaine public), l'intégrer dans `figures/`.

---

## 4. *Kith and kin* d'Archie Moore — cas limite extrême pour la Section VI

**Sources :**
- Article The Guardian : `https://www.theguardian.com/artanddesign/2024/apr/17/australia-venice-biennale-family-tree-kith-and-kin-archie-moore`
- Documentation panoramique officielle : `https://www.kithandkin.me/documentation/panoramic`

**Référence BibTeX :** `moore2024` — déjà dans `bibliography.bib`.

**Ce que c'est :** Une généalogie Aboriginal dessinée à la craie sur les murs et le plafond du Pavillon australien à la Biennale de Venise 2024, couvrant 65 000 ans de parenté. Le spectateur entre physiquement dans l'espace et se déplace pour naviguer l'arbre.

**Ce qu'il teste :** L'habitabilité *physique* (entrer dans l'espace avec son corps, se déplacer) se substitue-t-elle à l'habitabilité *structurelle* ? Le lecteur peut-il inférer des relations entre figures non adjacentes — ou ne fait-il que parcourir un arbre devenu très grand ?

**Relation avec Babenberg :** Ces deux cas forment une progression dans la Section VI :
- Babenberg : richesse spatiale et narrative dans un espace visuel 2D
- Archie Moore : transformation en espace physique tridimensionnel habitable

**Position dans le texte :** Section VI, comme cas limites les plus déstabilisants, après les cas qui tiennent (métro, bibliométrique) et avant la conclusion sur l'indétermination.

---

## 5. Métriques multiples — raffinement de la thèse

**Décision prise lors de la discussion (30 mai 2026) :**

La formulation initiale "une carte encode *une* métrique globale cohérente" est insuffisante. Une carte peut encoder **plusieurs métriques globales cohérentes simultanément**. Exemple : une carte des flux commerciaux encode à la fois une métrique spatiale (distances géographiques) et une métrique économique (volumes d'échanges). Chacune est globalement cohérente indépendamment.

**Implication pour la thèse :** Le créateur ne choisit pas seulement *quoi réduire*, il choisit *quelles dimensions de la réalité deviennent des métriques globalement cohérentes*. Chaque métrique encodée est une décision de conception.

**Cas du planisphère :** Un planisphère sans contenu thématique encode une seule métrique globale (la distance géographique), intrinsèque aux coordonnées. C'est probablement le cas le plus pur de carte. À démontrer proprement dans la Section II ou la Section VI.

**Cas "sans composante spatiale" :** Un réseau de flux commerciaux sans ancrage géographique est un graphe. Il devient une carte si et seulement si l'auteur impose un arrangement où la proximité visuelle encode une relation globalement cohérente. L'arrangement est l'acte cartographique.

**À intégrer dans :** Section II (métrique locale vs globale) — reformuler la définition pour inclure la possibilité de métriques multiples. Section V (synthèse) — préciser le rôle du créateur.

---

## 4. Cartogrammes — métriques hybrides et déformation intentionnelle

**Ce que c'est :** Un cartogramme est une carte géographique dans laquelle la surface (ou la distance) des entités est délibérément déformée pour être proportionnelle à une variable thématique — population, PIB, nombre de décès, etc.

**Pourquoi c'est important pour la thèse :** Le cartogramme est le cas où le créateur ne se contente pas d'*ajouter* une métrique thématique à une métrique spatiale — il *subordonne* la métrique spatiale à la métrique thématique. L'Afrique, massifiée par la population, occupe plus de surface que dans la réalité géographique. Le territoire géographique est sacrifié au profit de la lisibilité thématique.

**Ce qu'il teste :** Si la métrique spatiale peut être déformée jusqu'à ne plus correspondre à la réalité géographique, qu'est-ce qui fait encore de cela une carte ? La réponse probable : l'espace reste *globalement cohérent* — les pays restent voisins de leurs voisins réels, les continents restent reconnaissables, les relations de proximité sont préservées qualitativement même si elles sont quantitativement fausses. Le lecteur peut encore dériver des relations entre éléments non explicitement reliés.

**Lien avec Mercator :** La projection de Mercator déforme déjà les surfaces pour des raisons de navigation (les lignes droites = caps constants). Le cartogramme pousse cette logique à l'extrême : la déformation est *intentionnellement thématique*, pas un artefact de projection. Ce qui les rapproche : dans les deux cas, la carte assume la distorsion au service d'un message. Ce qui les distingue : dans Mercator, la métrique spatiale reste la métrique dominante (les directions sont préservées) ; dans le cartogramme, elle est explicitement secondarisée.

**Implication pour la définition :** Le créateur ne choisit pas seulement *quelles métriques encoder* — il choisit aussi leur *pondération relative*. Une carte peut faire primer une métrique thématique sur une métrique spatiale tout en restant une carte, à condition que l'espace reste globalement cohérent.

**Position dans le texte :** Section VI (tests) ou Section II, selon la profondeur de traitement souhaitée. Peut aussi renforcer la Section III (message et tension) : le cartogramme est peut-être l'exemple le plus pur de carte qui assume pleinement son message au détriment de la fidélité.

**Images disponibles :** Nombreux exemples domaine public ou CC sur Wikimedia Commons (recherche : "cartogram population", "worldmapper").

---

## Récapitulatif des actions

| Action | Priorité | Responsable |
|---|---|---|
| Choisir et télécharger image Babenberg (Wikimedia) | Section VI | Adrien |
| Prendre une capture de *Kith and kin* (ou utiliser lien) | Section VI | Adrien |
| Trouver image cartogramme CC (Wikimedia / Worldmapper) | Section VI ou II | Adrien |
| Reformuler définition métrique dans Section II (métriques multiples + pondération) | Rédaction | Claude |
| Intégrer Babenberg + Moore dans Section VI | Rédaction | Claude |
| Intégrer cartogrammes dans Section VI ou II | Rédaction | Claude |