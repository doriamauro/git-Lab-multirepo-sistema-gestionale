# Sistema gestionale - Laboratorio Git Submodule
# modifica
Repository integratore di due componenti Python sviluppati in repository indipendenti.

## Clonazione

```bash
git clone --recurse-submodules https://github.com/doriamauro/git-Lab-multirepo-sistema-gestionale.git
```

Se hai gia clonato il repository:

```bash
git submodule update --init --recursive
```

## Verifica dei riferimenti

```bash
git submodule status
git ls-tree HEAD
```

I due percorsi `gestione-ordini/` e `gestione-magazzino/` sono **gitlink** (modalita `160000`), non normali directory tracciate dal repository principale.

Ogni componente evolve autonomamente sul proprio `main`. Un nuovo commit del componente non aggiorna automaticamente il riferimento registrato qui.
