[![Deskargatu eLiburua](https://img.shields.io/badge/deskargatu-eBook%20PDF-blue?style=for-the-badge)](https://github.com/xezpeleta/sortu-dokumentazioa/releases/latest/download/sortu-dokumentazioa-github-erabiliz-light.pdf)

# Sortu eLiburu bat Markdown erabiliz
eLiburu bat modu kolaboratiboan sortzeko adibide soil bat da errepositorio hau.

[Markdown](https://en.wikipedia.org/wiki/Markdown) lengoaia erabiliz sortutako testu fitxategiak ondoren [eLiburu batean](https://github.com/xezpeleta/sortu-dokumentazioa/releases/latest/download/sortu-dokumentazioa-github-erabiliz-light.pdf) bihurtzen dira automatikoki, [Ibis](https://github.com/themsaid/ibis) proiektua eta GitHub Actions erabiliz.

## Ezaugarriak

- Sortu edukia testu hutseko fitxategietan (Markdown erabiliz)
- Aldaketak errez eta modu kolaboratiboan
- Bertsio kontrola, aldaketen historikoa
- Automatizatua, mantenurik gabekoa

Eta garrantzitsuena:
- Emaitza PDF gisa esportatu ahal izatea
  - Pertsonalizatutako azala jarrita
  - Automatikoki sortutako "Eduki taula"-rekin (klikablea)
  - Itxura aldagarria (tipografia, atzeko kolorea...)
  - Syntax highlighting

## Nola hasi?

Kopiatu errepositorio hau eta ondoren moldatu zure beharretara:
- Moldatu `ibis.php` fitxategia, bertan liburuari buruzko oinarrizko informazioa aurkituko duzu
- Moldatu liburuaren azala: `assets/cover.jpg` fitxategia ordezkatuz
- Sortu edukia: `./content` direktorioan fitxategiak sortuz

## PDF sorrera

Liburu honen azken bertsioa automatikoki sortzen da *"Release"* bat argitaratzen dugun bakoitzean.
