# Endurhönnun Upplýsingaverkfræði: Stigvaxandi þróun faglegra vinnubragða

**Helga Ingimundardóttir** ([ORCID 0000-0002-2780-3546](https://orcid.org/0000-0002-2780-3546))
Iðnaðarverkfræði-, vélaverkfræði- og tölvunarfræðideild (IVT), Háskóli Íslands

Ráðstefna Kennsluakademíu opinberu háskólanna, Veröld Háskóla Íslands, 20. nóvember 2026

- **Web version:** <https://tungufoss.github.io/Kennsluakademia-IDN302G/>
- **PDF:** [article.pdf](article.pdf)
- **Slides:** <https://tungufoss.github.io/Kennsluakademia-IDN302G/slides/> (placeholder, in progress)
- **Course website:** <https://hi-idn.github.io/IDN302G/>

## Útdráttur
Greinin lýsir endurhönnun Upplýsingaverkfræði með áherslu á hvernig kynna má fagleg vinnubrögð stigvaxandi snemma í námsleiðinni. Fjallað er um fræðilegan rökstuðning, uppbyggingu námskeiðsins, endurgjafarlotur og notkun sýnilegra ferlisgagna til að styðja þróun vinnubragða nemenda.

**Lykilorð:** upplýsingaverkfræði, rauntengt nám, fagleg vinnubrögð, stigvaxandi nám, leiðsagnarmat

## Vinsamlega vitnið í þetta verk sem
Ingimundardóttir, H. (2026). Endurhönnun Upplýsingaverkfræði: Stigvaxandi þróun faglegra vinnubragða. *Ráðstefna Kennsluakademíu opinberu háskólanna*, Veröld Háskóla Íslands, Reykjavík. <https://tungufoss.github.io/Kennsluakademia-IDN302G/>

```bibtex
@inproceedings{Ingimundardottir2026Kennsluakademia,
  author    = {Ingimundardóttir, Helga},
  title     = {Endurhönnun Upplýsingaverkfræði: Stigvaxandi þróun faglegra vinnubragða},
  booktitle = {Ráðstefna Kennsluakademíu opinberu háskólanna},
  address   = {Veröld Háskóla Íslands, Reykjavík},
  month     = nov,
  year      = {2026},
  url       = {https://tungufoss.github.io/Kennsluakademia-IDN302G/}
}
```

## Building
The paper is written once, in [article.qmd](article.qmd). [Quarto](https://quarto.org/) turns it into both the PDF and the web version:

```bash
quarto render article.qmd
```

This regenerates `article.tex`, `article.pdf` and `article.html`. Edit `article.qmd`, not `article.tex`, because every render overwrites it. Pushing to `main` publishes the web version (with the PDF) to GitHub Pages.

The slides are a Quarto RevealJS deck in [slides/index.qmd](slides/index.qmd), using the HÍ slide theme from [tungufoss/quarto-hi](https://github.com/tungufoss/quarto-hi). Render them with `quarto render slides/index.qmd`.

The figure is drawn in TikZ in [progressive_modules_figure.tikz](progressive_modules_figure.tikz). The PDF uses it directly; the web version uses [figures/progressive_modules.svg](figures/progressive_modules.svg), so if you change the figure, rebuild the SVG with the commands in [figures/progressive_modules_standalone.tex](figures/progressive_modules_standalone.tex).

The layout comes from the [Kennsluakademía conference template](https://github.com/HI-IDN/Conf-Kennsluakademia), which explains the setup in more detail.

## License
MIT, see [LICENCE](LICENCE).
