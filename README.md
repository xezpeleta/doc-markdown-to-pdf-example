# doc-markdown-to-pdf-example
Dokumentazioa sortzeko adibide bat besterik ez da errepositorio hau. [Markdown](https://en.wikipedia.org/wiki/Markdown) lengoaia erabiliz sortutako fitxategiak ondoren liburu itxurako PDF batean bihurtzen ditugu, [Ibis](https://github.com/themsaid/ibis) proiektua erabiliz.

Errepositorio honetako direktorio estruktura, hurrengo agindu honekin sortua izan da:


```bash
docker run -it --rm -v $(pwd):/data xezpeleta/ibis init
```

## Edizioa (aldaketak)
Dokumentazio honetan edonork egin ditzake aldaketak. Nahi izanez gero, baimenak kudeatu ahal izango genituzke eta pertsona zehatz batzueri baimendu aldaketak.

## PDF liburuaren argitaratzea
PDF fitxategia automatikoki eratzen da aldaketa bat egiten dugun bakoitzean. Horretarako Github Actions erabiltzen dugu.

PDF fitxategia zure ordenagailuan sortu nahi izanez gero, ondorengo aginduaren bidez ere sor genezake:

```bash
# Liburuaren itxura normala
ibis build

# Itxura iluna (dark theme)
ibis build dark

# Adibidezko "lagina" sortu nahi ezkero
ibis sample

# Lagina beltz itxurarekin
ibis sample dark
```

# Tests
aa
