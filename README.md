# Treenipäiväkirja

Oma treenisovellus salitreenien ja juoksujen kirjaamiseen. Toimii puhelimessa omalla kuvakkeellaan, koko näytöllä ja ilman nettiyhteyttä.

## Tiedostot

| Tiedosto | Mitä se tekee |
|---|---|
| `index.html` | Koko sovellus: ulkoasu (CSS) ja toiminta (JavaScript) |
| `manifest.webmanifest` | Kertoo puhelimelle sovelluksen nimen, kuvakkeen ja värit |
| `sw.js` | Service worker: tallentaa sovelluksen puhelimeen offline-käyttöä varten |
| `icons/` | Sovelluksen kuvakkeet |

## Julkaisu GitHub Pagesissa (ilmainen, n. 10 min)

Tee tämä mieluiten tietokoneella.

1. Luo tili osoitteessa github.com.
2. Valitse oikeasta yläkulmasta **+** ja sitten **New repository**. Anna nimeksi `treenit`, valitse **Public** ja paina **Create repository**.
3. Napauta sivulla linkkiä **uploading an existing file**. Pura zip-paketti ja raahaa kaikki tiedostot ja `icons`-kansio selaimeen. Paina **Commit changes**.
4. Avaa repositorion **Settings** ja sieltä vasemmalta **Pages**. Valitse kohtaan *Branch* `main` ja `/ (root)`, ja paina **Save**.
5. Odota minuutti tai kaksi. Sovellus on nyt osoitteessa `https://KÄYTTÄJÄNIMESI.github.io/treenit/`.

Repositorio on julkinen, joten koodi näkyy muille. Treenisi eivät näy, koska ne tallentuvat vain puhelimesi muistiin.

## Puhelimen kotinäytölle

**iPhone:** avaa osoite Safarissa, napauta Jaa-kuvaketta ja valitse **Lisää Koti-valikkoon**.

**Android:** avaa osoite Chromessa, avaa ⋮-valikko ja valitse **Asenna sovellus** (tai **Lisää aloitusnäytölle**).

Avaa sovellus jatkossa aina kotinäytön kuvakkeesta. Selaimessa avattu versio pitää omat tietonsa erillään.

## Tietojen tallessa pitäminen

- Treenit ovat puhelimen muistissa. Vie varmuuskopio silloin tällöin **Historia**-välilehden alareunasta.
- Puhelinta vaihtaessasi asenna sovellus uuteen puhelimeen ja valitse **Tuo varmuuskopio**.

## Kun muokkaat sovellusta

1. Tee muutokset `index.html`-tiedostoon.
2. Nosta `sw.js`-tiedoston alussa versionumeroa, esim. `treenit-v1` → `treenit-v2`. Muuten puhelin käyttää vanhaa tallennettua versiota.
3. Lataa muuttuneet tiedostot GitHubiin samalla tavalla kuin kohdassa 3.
4. Sulje sovellus puhelimessa ja avaa se uudelleen, tarvittaessa kahdesti.
