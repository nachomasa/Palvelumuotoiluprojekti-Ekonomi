# dumppiryekonomi – Dumppi ry:n mobiilisovelluksen demo

Staattinen esittelysivu (HTML/CSS/JS), jossa Dumppi ry:n mobiilisovellus toimii klikattavana demona.
Kirjautuminen onnistuu millä tahansa tunnuksella. Tiedot eivät tallennu, vaan ne nollautuvat sivun päivityksessä.

## Julkaisu GitHub Pagesissa
1. Luo GitHubissa uusi repository, esim. `dumppiryekonomi`.
2. Lataa kaikki tämän kansion tiedostot repositoryn juureen (`index.html`, `assets/`, `.nojekyll`, `README.md`).
3. Avaa **Settings → Pages**, valitse **Deploy from a branch**, branch `main` ja kansio `/ (root)`.
4. Hetken päästä sivu aukeaa osoitteessa `https://KÄYTTÄJÄ.github.io/dumppiryekonomi/`.

## Rakenne
- `index.html` – koko sovellus (tyylit ja skriptit samassa tiedostossa)
- `assets/dumppi-logo.png` – Dumppi ry:n logo (vaihda tähän virallinen tiedosto samalla nimellä)

## Live-keskustelu (Firebase)
Foorumin viestit näkyvät kaikille 10 minuuttia. Jokainen käyttäjä (anonyymi Firebase-tunnus) voi lähettää yhden viestin kerrallaan.
1. Firebase Console → Authentication → Sign-in method → ota käyttöön **Anonymous**.
2. Realtime Database → Rules → liitä tiedoston `firebase-rules.json` sisältö ja paina Publish.
3. Firebase-asetukset ovat `index.html`-tiedoston lopussa (`const cfg`).
