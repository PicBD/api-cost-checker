# 🎨 API Cost Checker

**Outil de mesure des coûts API réels vs théoriques**  
Conçu pour [PicBD](https://github.com/PicBD) · Utilisable pour tout projet IA générative

🔗 **[Ouvrir l'application](https://picbd.github.io/api-cost-checker/)**

---

## À quoi ça sert ?

Quand on développe une application qui utilise des API d'IA générative (images, texte), il est impossible de fixer un barème de prix ou de crédits sans connaître les **vrais coûts de génération**.

Ce projet fournit une checklist interactive pour :

- Mesurer le **coût réel relevé dans l'API Ledger** pour chaque type de génération
- Le comparer au **coût théorique calculé** à partir des tarifs officiels
- Calculer l'**écart en %** entre les deux
- Produire des **moyennes par type de création** exploitables pour fixer un barème

## Cas d'usage

Conçu initialement pour mesurer les coûts de génération de PicBD (application iOS de création de BD personnalisées par IA), cet outil est générique et utilisable pour **tout projet facturant des générations IA** :

- Applications de génération d'images
- Chatbots et assistants IA
- Générateurs de contenu texte
- Outils créatifs propulsés par Gemini, OpenAI, Anthropic, etc.

## Fonctionnalités

- ✅ **12 tests structurés** (4 types × 3 variantes)
- ✅ **Saisie du coût réel Ledger** (valeur clé)
- ✅ **Calcul automatique** de l'écart réel / théorique
- ✅ **Progression sauvegardée** automatiquement dans le navigateur
- ✅ **Résumé exportable** en un clic
- ✅ **100% standalone** — aucune installation, aucune dépendance
- ✅ **Responsive** — fonctionne sur mobile et desktop

## Utilisation

### En ligne
👉 **[https://picbd.github.io/api-cost-checker/](https://picbd.github.io/api-cost-checker/)**

### En local
1. Télécharger `index.html`
2. Double-cliquer pour l'ouvrir dans n'importe quel navigateur
3. La progression est sauvegardée localement (localStorage)

### Avec le classeur Excel
L'outil est conçu pour fonctionner en parallèle avec le classeur Excel `PicBD_Grille_tests_couts.xlsx` :
1. Remplir les champs dans la checklist
2. Reporter les valeurs dans la ligne Excel correspondante (indiquée dans chaque test)
3. Le classeur calcule automatiquement les moyennes et le barème de crédits

## Structure des tests

| Type | Variantes | Ligne Excel |
|------|-----------|-------------|
| Mural | 1, 2, 3 personnages | 6, 7, 8 |
| BD courte | 1, 2, 3 personnages | 9, 10, 11 |
| BD moyenne | 1, 2, 3 personnages | 12, 13, 14 |
| BD longue | 1, 2, 3 personnages | 15, 16, 17 |

## Tarifs de référence (juin 2026)

Les calculs théoriques sont basés sur :
- **Image** : 0,067 $/image (Gemini 3.1 Flash Image)
- **Texte entrée** : 1,50 $/M tokens (Gemini 3.5 Flash)
- **Texte sortie** : 9,00 $/M tokens (Gemini 3.5 Flash)

> ⚠️ Les tarifs IA évoluent rapidement. Toujours vérifier sur la documentation officielle du fournisseur.

## Licence

MIT License © 2026 Stéphane SAULNIER

Permission is hereby granted, free of charge, to any person obtaining a copy of this software to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software, subject to the following conditions: the above copyright notice and this permission notice shall be included in all copies or substantial portions of the software.
