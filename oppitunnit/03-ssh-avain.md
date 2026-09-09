---
title: 3. SSH-avaimen käyttäminen
parent: Oppitunnit
nav_order: 3
---

# SSH-avaimen käyttäminen

📺 [Katso opetusvideo](https://esedu.sharepoint.com/:v:/r/sites/Koodarit562/Luokan%20materiaali/OHJ2-Git-Github/03-git-github-ssh-keygen.webm?csf=1&web=1&e=MsOcDI)

## Sisältö

- SSH-avainparin luominen
- SSH-avaimen lisääminen GitHubiin
- SSH-yhteyden testaaminen

## SSH-avainparin luominen

Luo SSH-avainpari komennolla:

```bash
ssh-keygen -t ed25519 -C "sahkoposti@esimerkki.com"
```

    Seuraa komentorivin ohjeita. Voit yleensä hyväksyä oletuspolun ja jättää salasanan tyhjäksi, ellei sinulla ole erityistä syytä käyttää salasanaa. SSH-avainpari tallennetaan yleensä kotihakemistoosi kansioon `~/.ssh/`.
    Voit tarkistaa, että avaimet on luotu onnistuneesti komennolla:

    ```bash
    ls ~/.ssh/
    ```

    Sinun pitäisi nähdä tiedostot `id_ed25519` (yksityinen avain) ja `id_ed25519.pub` (julkinen avain) listattuna.

    Nyt sinulla on SSH-avainpari, jota voit käyttää GitHubin kanssa. Seuraavaksi lisätään julkinen avain GitHubiin.

## SSH-avaimen lisääminen GitHubiin

1. Kopioi julkisen avaimen sisältö komennolla:

    ```bash
    cat ~/.ssh/id_ed25519.pub
    ```

2. Kirjaudu GitHubiin ja siirry kohtaan **Settings > SSH and GPG keys**.
3. Klikkaa **New SSH key**, liitä kopioitu avain kenttään ja tallenna.

## SSH-yhteyden testaaminen

Testaa, että SSH-yhteys GitHubiin toimii komennolla:

```bash
ssh -T git@github.com
```

Jos kaikki on kunnossa, sinun pitäisi nähdä viesti, joka kertoo onnistuneesta todennuksesta. Esimerkiksi:

```
Hi käyttäjänimi! You've successfully authenticated, but GitHub does not provide shell access.
``` 

