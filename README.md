# Git ja GitHub -kurssin verkkosivut

Tämä on kurssimateriaalisivusto, joka on toteutettu **Markdownilla** ja julkaistaan **GitHub Pagesissa** (Jekyll + [just-the-docs](https://just-the-docs.com/) -teema). Sivusto on suunniteltu niin, että uuden oppitunnin lisääminen vaatii vain yhden uuden `.md`-tiedoston.

## Sivuston rakenne

```
├── _config.yml          # Sivuston asetukset (teema, otsikko, jne.)
├── index.md              # Etusivu
└── oppitunnit/
    ├── index.md          # "Oppitunnit"-valikon yläsivu
    ├── 01-git-ja-github.md
    ├── 02-gitin-asennus.md
    ├── 03-ssh-avain.md
    ├── 04-git-init-clone.md
    └── 05-git-status-log-diff.md
```

## Uuden oppitunnin lisääminen

1. Luo `oppitunnit/`-kansioon uusi tiedosto, esim. `06-oma-otsikko.md`.
2. Kopioi tiedoston alkuun tämä "front matter" -osio ja täytä tiedot:

   ```yaml
   ---
   title: 6. Oman oppitunnin otsikko
   parent: Oppitunnit
   nav_order: 6
   ---
   ```

3. Kirjoita sisältö tiedoston loppuosaan tavallisella Markdownilla, esim.:

   ```markdown
   # Oman oppitunnin otsikko

   📺 [Katso opetusvideo](https://linkki-videoon)

   ## Sisältö

   - Asia 1
   - Asia 2
   ```

4. Tallenna, commitoi ja pushaa GitHubiin (`git add`, `git commit`, `git push`) — sivusto päivittyy automaattisesti muutaman minuutin kuluessa.

Sivun ei tarvitse muistaa lisätä linkkiä mihinkään - **valikko vasemmassa reunassa muodostuu automaattisesti** `nav_order`-kentän perusteella.

## Sivuston julkaiseminen GitHub Pagesissa (kerran tehtävä alkuasetus)

1. Luo GitHub-repositorio ja pushaa tämän kansion sisältö sinne.
2. Mene repositorion **Settings → Pages**.
3. Valitse **Source: Deploy from a branch**, branch: `main`, kansio `/ (root)`.
4. Tallenna. Sivusto ilmestyy hetken kuluttua osoitteeseen `https://KAYTTAJATUNNUS.github.io/REPON-NIMI/`.
5. Päivitä [_config.yml](_config.yml)-tiedostoon oikeat `url` ja `baseurl`-arvot sekä `gh_edit_repository`-linkki vastaamaan omaa repositoriotasi.

## Esikatselu omalla koneella (valinnainen)

Jos haluat nähdä muutokset ennen julkaisua:

```bash
bundle install
bundle exec jekyll serve
```

Sivusto aukeaa osoitteessa `http://localhost:4000`.

> Huom: Sivuston sharepoint-videot vaativat kirjautumisen organisaation tunnuksilla, joten linkit toimivat vain oppilaitoksen käyttäjille.
