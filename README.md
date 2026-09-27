# Marxisterna.se

En svenskspråkig webbplats för den politiska föreningen Marxisterna, byggd med [Hugo](https://gohugo.io/) och förberedd för GitHub Pages.

All synlig text är tills vidare exempeltext. De röda och vita logotyperna i `static/images/` är föreningens egna originalfiler.

## Köra webbplatsen lokalt

Installera Hugo 0.166.0 eller senare och kör:

```sh
hugo server
```

Öppna sedan adressen som Hugo visar i terminalen.

## Redigera innehåll

- Startsidan finns i `layouts/index.html`.
- Sidorna Om oss, Vår politik och Engagera dig finns i `content/`.
- Blogginlägg finns i `content/blogg/`.
- Färger, typografi och layout finns i `assets/css/main.css`.

## Publicering

Arbetsflödet i `.github/workflows/hugo.yaml` bygger och publicerar webbplatsen automatiskt när en ändring skickas till grenen `main`.

I repositoryts inställningar behöver **Settings → Pages → Source** vara satt till **GitHub Actions**. Filen `static/CNAME` är förberedd för domänen `marxisterna.se`; domänens DNS-poster måste också peka på GitHub Pages innan adressen fungerar.

