tests
# Biblio
Une petite application en ligne de commande pour gérer une bibliothèque : consulter le catalogue, rechercher un livre, enregistrer les emprunts et retours, et repérer les retards.

## Prérequis

| Python | 3.8 ou supérieur | `python --version` | linux : sudo apt isntall python3 | Windows : winget install -e --id Python.Python.3.12 | 
| MacOs : brew install python |
| SQLite (module `sqlite3`) | inclus avec Python | `python -c "import sqlite3; print(sqlite3.sqlite_version)"` |


## Installation

Aucune dépendance à installer.
Bibliothèque Python standard uniquement.

### macOS / Linux

```bash
git clone https://github.com/ANome1/biblio-groupe-Baptiste-Ilian-Nome.git
cd biblio-groupe-Baptiste-Ilian-Nome
python3 biblio.py init
```

### Windows

```powershell
git clone https://github.com/ANome1/biblio-groupe-Baptiste-Ilian-Nome.git
cd biblio-groupe-Baptiste-Ilian-Nome
py biblio.py init
```

Résultat attendu :

```text
Base initialisee : 6 livres, 3 membres.
```

## Commandes

Exécutez les commandes depuis le dossier du projet.

| Commande | Description |
| --- | --- |
| `python biblio.py init` | Remet les données de départ. |
| `python biblio.py livres` | Liste tous les livres, disponibles ou empruntés. |
| `python biblio.py chercher <texte>` | Recherche un livre par titre. |
| `python biblio.py emprunter <livre> <membre>` | Enregistre l’emprunt d’un livre par un membre. |
| `python biblio.py rendre <livre>` | Enregistre le retour d’un livre. |
| `python biblio.py retards` | Liste les livres empruntés depuis plus de 14 jours et non rendus.

## Exemples

Afficher le catalogue :

```bash
python biblio.py livres
```

Rechercher les livres dont le titre contient « harry » :

```bash
python biblio.py chercher harry
```

Enregistrer un emprunt :

```bash
python biblio.py emprunter "Le Petit Prince" Alice
```

Enregistrer un retour :

```bash
python biblio.py rendre "Le Petit Prince"
```

Afficher les retards :

```bash
python biblio.py retards
```

## Réinitialiser les données

Pour revenir aux données de démonstration, relancez :

```bash
python biblio.py init
```

> Cette commande réinitialise les données existantes.

