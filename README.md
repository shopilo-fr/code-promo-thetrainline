# Code promo Trainline, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Trainline** depuis [shopilo.fr](https://shopilo.fr/reductions/thetrainline.com). Renvoie les **coupons Trainline** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-thetrainline](https://shopilo-fr.github.io/code-promo-thetrainline/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-thetrainline
cd code-promo-thetrainline
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Trainline",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur les billets de train europeens",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/thetrainline.com"
  }
]
```

## Coupons Trainline disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur les billets de train europeens | [shopilo.fr](https://shopilo.fr/reductions/thetrainline.com) |

Codes actifs : **[shopilo.fr/reductions/thetrainline.com](https://shopilo.fr/reductions/thetrainline.com)**

## Questions frequentes

### Comment utiliser un code promo Trainline ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/thetrainline.com), ajoutez les produits a votre panier sur Trainline et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Trainline ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Trainline les plus recents ?
La page [shopilo.fr/reductions/thetrainline.com](https://shopilo.fr/reductions/thetrainline.com) est mise a jour quotidiennement avec les codes promo Trainline, bons de reduction Trainline et coupons promotionnels Trainline les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Trainline

Trainline est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/thetrainline.com), retrouvez les meilleurs codes promo Trainline, coupons Trainline verifies et bons de reduction Trainline actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-thetrainline
```

```javascript
const { fetchCoupons } = require('code-promo-thetrainline');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
