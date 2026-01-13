# Fork info

Copie de la bibliothèque [dibisoplot](https://github.com/dibiso-upsaclay/dibisoplot) pour adaptation locale.

branche main -> traque le repo d'origine (DiBISO/Université Paris-Saclay)
branche dbist -> modifications effectuées par l'équipe de la DBIST/UVSQ.

## Liste des changements

1. format des figures produites : passage de tex à html et de pdf à png
2. légères modifications du format des cartes
3. Pour des raisons de configuration locale d'environnement de travail (= Windows), les versions des bibliothèques plotly et kaleido ont dû être modifiées à la fois pour dibisoplot et dibisoreporting. La configuration suivante fonctionne sans dommage apparent : 
- plotly 6.3.1
- kaleido 1.1.0 
- openalex-analysis 0.15.2, malgré une erreur de compatibilité avec kaleido signalée par pip, sans conséquence notable
Les fichiers requirements.txt et pyproject.toml ont été mis à jour en conséquence.

## TO DO

- [ ] refondre les noms des fonctions encore marquées par LaTeX
- [ ] dé-LaTeXiser les messages d'erreurs, fallbacks, etc => simplification générale 
- [ ] faire pour pubpart le travail effectué sur biso

---

Original description below

---

# DiBISO plot

A Python library for plotting bibliometric research data, developed at the [DiBISO](https://www.bibliotheques.universite-paris-saclay.fr/en/department-libraries-information-and-open-science-dibiso-and-its-missions).

For more details about this project, you can read our [technical report](https://universite-paris-saclay.hal.science/hal-05336463).

Install with:

```bash
pip install dibisoplot
```

The library contains the following submodules:

  - `biso`: plot data for the BiSO (Open-Science Report)
  - `pubpart`: plot data about publications and partnerships


Homepage: https://pypi.org/project/dibisoplot/

Documentation: https://dibiso-upsaclay.github.io/dibisoplot/

Repository URL: https://github.com/dibiso-upsaclay/dibisoplot

Repository DOI: https://doi.org/10.5281/zenodo.17251536

Technical report: https://universite-paris-saclay.hal.science/hal-05336463


## About the BiSO

The BiSO (Bilan Science Ouverte - Open Science Report) is an annual report produced for each research laboratory under 
the responsibility of the Open Science teams (DiBISO) at Université Paris-Saclay. 
Prepared in collaboration with the laboratories, it is based on open data, mainly coming from the [HAL](https://hal.science/) repository but 
also from [OpenAlex](https://openalex.org/), [scanR](https://scanr.enseignementsup-recherche.gouv.fr/) and the [BSO](https://barometredelascienceouverte.esr.gouv.fr/). 
The BiSO presents indicators such as publication types, open access rates, and collaborations. 
Primarily intended for the laboratories under our scope, the report supports the development of open science practices. 
The code and template are shared under open-source licenses, allowing other institutions to reuse and adapt the 
methodology.

## About the Publications and Partnerships

This submodule uses data from [OpenAlex](https://openalex.org/) to make plots about publication topics, institutions, and citations, as 
well as common publication topics and potential collaboration topics with other institutions.

Romain THOMAS 2025  
Department of Libraries, Information and Open Science (DiBISO)  
Université Paris-Saclay