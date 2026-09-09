---
title: 5. Gitin peruskomentoja - commit
parent: Oppitunnit
nav_order: 5
---

# Commitin tekeminen

📺 [Katso opetusvideo](https://esedu.sharepoint.com/:v:/r/sites/Koodarit562/Luokan%20materiaali/OHJ2-Git-Github/06-git-status-log-diff.webm?csf=1&web=1&e=ui0jVq)

## Sisältö

- `git commit` - muutosten tallentaminen paikalliseen repositorioon
- `git add` - muutosten lisääminen vaiheistettuun alueeseen ennen commitin tekemistä
- `git status` - muutosten tilan tarkastelu

## Gitin työskentelyalueet

Gitin työskentelyalueet voidaan jakaa kolmeen osaan:

- **Työskentelyalue (Working Directory)**: Paikka, jossa teet muutoksia tiedostoihin.
- **Vaiheistettu alue (Staging Area)**: Alue, johon lisäät muutokset ennen commitin tekemistä (`git add`).
- **Paikallinen repositorio (Local Repository)**: Paikka, johon commitit tallennetaan (`git commit`).

![Gitin työskentelyalueet: working directory, staging area ja repository]({{ "/assets/images/git-workflow.png" | relative_url }})

## Gitin peruskomennot

### git add

`git add` -komennolla lisätään muutokset vaiheistettuun alueeseen ennen commitin tekemistä. Esimerkiksi:

```bash
git add <tiedosto>
```

### git commit

`git commit` -komennolla tallennetaan muutokset paikalliseen repositorioon. Esimerkiksi:

```bash
git commit -m "Kuvaava viesti commitista"
```

### git status

`git status` -komennolla voidaan tarkastella muutosten tilaa:

```bash
git status
```
