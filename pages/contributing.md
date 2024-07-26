---
title: Contributing
---

## Creating your own How-to Guide

{% include callout.html type="important" content="Want to create your own How-to Guide? See [this guide](https://australianbiocommons.github.io/how-to-guide-template/) for more information." %}


## Adding a How-to Guide to the Hub


If you have prepared a How-to Guide that is related to a BioCommons activity, we invite you to add it to the How-to Hub. Please check that your guide meets our suggested standards, including:

- The guide is [FAIR (findable, accessible, interoperable, and reusable)](https://doi.org/10.1038/sdata.2016.18)
- All contributors are acknowledged
- The guide is relevant to a national audience
- The guide provides enduring access to digital technique(s), data or tool(s) needed to conduct world class research

{% include callout.html type="important" content="A guide does not necessarily need to use the How-to Guide template to be included in the How-to Hub. If you have an existing guide in your own format, skip to step 3. If you are unsure about whether your guide is suitable, please [contact us](https://www.biocommons.org.au/contact-form)." %}


If you answered yes above, follow this process:

1. Create a How-to Guide using our [How-to Guide for creating a How-to Guide](https://australianbiocommons.github.io/how-to-guide-template/).
2. Make sure your guide has the following:
   - A completed `CITATION.cff` file
   - All included sections should be completed, in particular the main index page, which contains the following sections: `About`, `Please cite this guide as follows`, `Acknowledgements` and `References`.
   - An up-to-date `CONTRIBUTORS.yml` file 
   - A `Back to How-to Hub` button in the top navigation panel of your How-to Guide (see example snippet below that needs to be added to the `_data/topnav.yml` file)

```yaml
- title: Back to How-to Hub
  url: https://australianbiocommons.github.io/how-to-hub/index
```

{:start="3"}
3. Fork the How-to Hub repository: [https://github.com/AustralianBioCommons/how-to-hub/fork](https://github.com/AustralianBioCommons/how-to-hub/fork)
4. Add your guide to the How-to Hub by adding the following `yaml` snippet to the How-to Hub `_data/tool_and_resource_list.yml` file.

```yaml
- id: page_identifier
  description: Add a meaningful description for your How-to Guide here.
  url: Add the URL for your How-to Guide here.
  name: Add the title of your How-to Guide here.
  related_pages:
    - Add the category identifier for the page. This determines which How-to Hub category page your guide appears on.
```

A completed example is available below: 

```yaml
- id: genome-assembly-hifi
  description:
    This How-to Guide describes the steps required to assemble your genome on the Galaxy Australia platform, using multiple workflows developed in consultation between the Bioplatforms Australia Threatened Species Initiative, Galaxy Australia, and the Australian BioCommons.
  url: https://australianbiocommons.github.io/how-to-guides/genome_assembly/hifi_assembly
  name: Genome assembly with `hifiasm` on Galaxy Australia
  related_pages:
    - genome_assembly
```

{:start="5"}
5. Generate a pull request (PR) against the main branch of the How-to Hub.
6. Hub maintainers will review your PR and approve the guide, or make some suggestions for changes.
7. Once any suggested changes have been addressed, the PR will be merged and your guide will be part of the How-to Hub listing.


## Editing the How-to Hub

### GitHub issues

If you think something should be added, or if you find an error, bug or mistake, please [create an issue](https://github.com/AustralianBioCommons/how-to-hub/issues) detailing the problem. We will do our best to fix the issue as soon as possible. You can also create an issue by clicking the `!` symbol next to the title on any of the pages.


### Pull Request

If you want to edit content on this site, please do the following:

1. Please let us know via GitHub [issues](https://github.com/AustralianBioCommons/how-to-hub/issues).
2. Create your own fork of this GitHub repository.
3. In your fork, create a branch with a concise name, that reflects its contents (e.g. `add/how-to-login-galaxy`).
4. Make sure you update [`CONTRIBUTORS.yml`](https://github.com/AustralianBioCommons/how-to-hub/blob/main/_data/CONTRIBUTORS.yml).
5. Create and commit the edits to your new branch.
6. Open a GitHub Pull Request (PR) on this repository for your branch, concisely providing context for your additions.
7. Follow-up on any feedback from the repository maintainers.
8. Once ready, the maintainers will merge the changes and deploy the new content.


## Thanks for contributing!
