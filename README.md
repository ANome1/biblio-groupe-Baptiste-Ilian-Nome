# Biblio
Une petite application en ligne de commande pour gérer une bibliothèque : consulter le catalogue, rechercher un livre, enregistrer les emprunts et retours, et repérer les retards.

## Prérequis



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

