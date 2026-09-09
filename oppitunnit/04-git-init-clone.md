---
title: 4. Git init ja clone
parent: Oppitunnit
nav_order: 4
---

# Git init ja clone

📺 [Katso opetusvideo](https://esedu.sharepoint.com/:v:/r/sites/Koodarit562/Luokan%20materiaali/OHJ2-Git-Github/04-git-init-clone.webm?csf=1&web=1&e=55eQpq)

## Sisältö

- Mikä on Git-repositorio?
- Uuden repositorion luominen (`git init`)
- Olemassa olevan repositorion kloonaaminen (`git clone`)
- Paikallisen ja etärepositorion ero

## Mikä on Git-repositorio?

Git-repositorio on paikka, jossa Git tallentaa projektin historian ja muutokset. Se sisältää kaikki tiedostot, commitit ja haarat, jotka mahdollistavat projektin versionhallinnan. Repositorio voi olla paikallinen (omalla koneellasi) tai etäinen (esim. GitHubissa).

## Uuden repositorion luominen (`git init`)

Uuden Git-repositorion luominen paikalliselle koneelle onnistuu komennolla:

```bash
git init
```

Tämä komento luo uuden `.git`-kansion nykyiseen hakemistoon, mikä tekee siitä Git-repositorion. Voit tämän jälkeen lisätä hakemistoon tiedostoja ja tehdä ensimmäisen commitin. Commitin tekemisestä on enemmän seauraavassa luvussa.

## Olemassa olevan repositorion kloonaaminen (`git clone`)

Jos haluat työskennellä olemassa olevan Git-repositorion kanssa paikallisesti, voit kloonata sen komennolla:

```bash
git clone <repository-url>
```

Tämä komento luo uuden hakemiston, jossa on kopio etärepositoriosta. Voit tämän jälkeen tehdä muutoksia paikallisesti ja työntää ne takaisin etärepositorioon.

## Paikallisen ja etärepositorion ero

- **Paikallinen repositorio**: Repositorio, joka sijaitsee omalla koneellasi. Voit tehdä muutoksia ja committeja ilman internet-yhteyttä.
- **Etärepositorio**: Repositorio, joka sijaitsee palvelimella (esim. GitHubissa). Paikalliset muutokset voidaan työntää etärepositorioon (`git push`) ja etärepositorion muutokset voidaan hakea paikalliseen repositorioon (`git pull`).

