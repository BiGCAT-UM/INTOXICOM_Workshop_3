# BioHackrXiv Template for INTOXICOM Workshop Reports

Minimal example of a [BioHackrXiv](https://biohackrxiv.org/) publication that can be generated with the
[Preview Service](http://preview.biohackrxiv.org/) for an
[INTOXICOM](https://elixir-europe.org/internal-projects/commissioned-services/integrating-toxicology-community) Workshop Report.
Each of the workshops will write one report.

## Step 1: Clone this Template Repository

This repository is a template repository. This means that you can hit the green "Use this template"
button (after logging in) to use it as a template to start a new BioHackrXiv Publication:

![Screenshot of the green "Use this template" button.](paper/use-this-template.png)

## Step 2: Configuring the Markdown

The publication Markdown is found in the `paper/paper.md` file. At the top you can edit the
YAML code with metadata. It is important to get this part correct, because otherwise the PDF
generation will fail. The metadata looks like this:

```yaml
title: 'INTOXICOM Workshop Report: Shedding the light on unknown chemical substances'
title_short: 'INTOXIOM #1: unknown chemical substances'
tags:
  - toxicology
  - PubChem
  - unknown chemical substances
authors:
  - name: Marvin Martens
    affiliation: 1
affiliations:
  - name: Dept of Bioinformatics - BiGCaT, NUTRIM, FHML, Maastricht University, Maastricht, NL
    index: 1
date: 7 November 2022
cito-bibliography: paper.bib
event: INTOXICOM
biohackathon_name: "INTOXICOM Workshops"
biohackathon_url:   "https://elixir-europe.org/internal-projects/commissioned-services/integrating-toxicology-community"
biohackathon_location: "Basel, Switserland, 2024"
group: Workshop 1
# URL to project git repo --- should contain the actual paper.md:
git_url: https://github.com/biohackrxiv/publication-template
# This is the short authors description that is used at the
# bottom of the generated paper (typically the first two authors):
authors_short: Martens \emph{et al.}
```

### Which metadata to update?

#### To change

The following fields should be changed:

* title
* title_short
* tags
* authors
* affiliations
* date
* group
* authors_short

Particularly important to update is the following field, which should point to
your clone of the template, instead of the template itself:

* git_url: https://github.com/biohackrxiv/publication-template

#### Only update for other BioHackathons

The following fields should only be changed if you are not writing for the INTOXICOM Workshops:

* event: INTOXICOM
* biohackathon_name: "INTOXICOM Workshops"
* biohackathon_url:   "[https://biohackathon-europe.org/](https://elixir-europe.org/internal-projects/commissioned-services/integrating-toxicology-community)"
* biohackathon_location: "Europe, 2024-2025"

## Step 3: Writing the article

A full Markdown example is given in [paper/paper.md](paper/paper.md). This includes instructions how to include
figures, tables, and annotate citations with the Citation Typing Ontology.

## Step 4: Previewing the paper as PDF

This repository can be converted into a preview PDF with BioHackrXiv [Preview Server](http://preview.biohackrxiv.org/).
The preview website asks for the link to your repository and will automatically find the `paper.md` and create an PDF.

