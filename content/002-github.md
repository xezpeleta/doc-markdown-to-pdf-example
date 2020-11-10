# GitHub

GitHub lankidetza garapen plataforma bat da. Azpitik Git bertsio kontrolerako sistema erabiltzen du.

Honi esker dokumentazioa sortu ahal izango dugu lantalde bateko kide ezberdinen artean. Gainera, software garapenean erabiltzen diren hainbat tresna erabiltzeko aukera ere izango ditugu.

## GitHub erabiltzen

### Erabiltzaile kontua

Atal honetan erabiltzailea nola sortu azalduko dugu

### Nola sortu errepositorioa

Beste atal honetan, Fork egin eta hasierako aldaketak nola egin azalduko dugu

## Github Actions

>{notice} Atal honetan lan fluxu honen tripak azaltzen dira. Ez da beharrezkoa hurrengo hau ulertzea liburu honetan aldaketak egiteko.

Errepositorio honek Github Actions erabiltzen du PDF fitxategia automatikoki eratzeko. Horretarako dago workflow hau `.github/workflows/main.yml`:

```yaml
on:
  push:
    tags:
      - '*'

name: Build Ibis eBook PDF

jobs:
  build:
    name: Build Ibis eBook PDF
    runs-on: ubuntu-latest
    steps:
      - name: Check out code
        uses: actions/checkout@v2
      - name: Build PDFs
        run: |
          docker run --rm -v ${{ github.workspace }}:/data xezpeleta/ibis:latest build
      - name: Upload release binaries
        uses: alexellis/upload-assets@0.2.2
        env:
          GITHUB_TOKEN: ${{ github.token }}
        with:
          asset_paths: '["./export/*"]'   
```

Fitxategi hau aldatu gabe utzi daiteke. Baina aitzaki bezala erabili dut *syntax highliting* ezaugarria probatzeko liburu honetan :)


