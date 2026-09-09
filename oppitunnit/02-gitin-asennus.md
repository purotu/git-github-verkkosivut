---
title: 2. Gitin asennus ja käyttöönotto
parent: Oppitunnit
nav_order: 2
---

# Gitin asennus ja käyttöönotto

📺 [Katso opetusvideo](https://esedu.sharepoint.com/:v:/r/sites/Koodarit562/Luokan%20materiaali/OHJ2-Git-Github/02-gitin-asennus.webm?csf=1&web=1&e=dcWGBD)

## Sisältö

- Gitin asentaminen omalle koneelle
- Gitin perusasetukset (nimi, sähköposti)
- Käyttöönoton tarkistaminen

## Gitin asentaminen Windowsille

Asenna Git Windowsille lataamalla asennusohjelma osoitteesta [https://git-scm.com/download/win](https://git-scm.com/download/win) ja seuraamalla asennusohjelman ohjeita. Voit hyväksyä oletusasetukset useimmissa kohdissa.

## Gitin asentaminen macOS:lle

Asenna Git macOS:lle käyttämällä Homebrew'ta komennolla:

```bash
brew install git
```

Vaihtoehtoisesti voit ladata asennusohjelman osoitteesta [https://git-scm.com/download/mac](https://git-scm.com/download/mac) ja seurata ohjeita.

## Gitin asentaminen Linuxille

Asenna Git Linuxille käyttämällä jakelusi pakettienhallintaa. Esimerkiksi Ubuntu/Debian-järjestelmissä komento on:

```bash
sudo apt update
sudo apt install git
```

## Gitin perusasetukset

Kun Git on asennettu, määritä käyttäjänimesi ja sähköpostiosoitteesi komentoja käyttäen:

```bash
git config --global user.name "Oma Nimesi"
git config --global user.email "sahkoposti@esimerkki.com"
```

## Käyttöönoton tarkistaminen

Varmista, että Git on asennettu ja asetukset ovat oikein komennolla:

```bash
git --version
git config --list
```