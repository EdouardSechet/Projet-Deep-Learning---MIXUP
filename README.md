# Projet-Deep-Learning---MIXUP
Ce projet explore l'implémentation et les effets de la technique d'augmentation de données Mixup sur le dataset CIFAR-10.

# Contexte et théorie
Le Mixup est une forme d'apprentissage vicinal qui encourage les modèles de réseaux de neurones à se comporter de manière linéaire entre les exemples d'entraînement.

## Références
Le détail des articles de recherche (Zhang, Wu, Verma) est disponible dans le dossier [`papiers/`](./papiers/).

# Résultats (CIFAR - 10)
Comparaison d'un CNN entrainé avec et sans mixup sur 20 et 50 epochs.

| Configuration | Époques | Précision (Accuracy) |
| :--- | :---: | :---: |
| **Standard (ERM)** | 20 | 72.38% |
| **Mixup ($\alpha=0.2$)** | 20 | **78.46%** |
| --- | --- | --- | --- |
| **Standard (ERM)** | 50 | 78.81% |
| **Mixup ($\alpha=0.2$)** | 50 | **79.41%** |

Note : On observe une convergence plus rapide et une meilleure robustesse face au surapprentissage avec le Mixup.

# Installation des dépendances
```bash
pip install -r requirements.txt
