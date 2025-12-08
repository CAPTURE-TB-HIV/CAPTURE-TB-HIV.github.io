# CAPTURE

This repository hosts the Jekyll website served at **https://capture-tb-hiv.github.io/**.

## Requirements
* npm
* Jekyll: https://jekyllrb.com/docs/installation/

## Serving locally
When first building the site, run `npm install` to install [Bootstrap](https://getbootstrap.com/).
Run `jekyll serve` to build the site locally. 

Open <http://localhost:4000> in your browser to preview the site.

## Updating content

- To add a **news item**, edit the yaml in `data/news.yaml`
- To add or edit a **person**, upload any photos to `assets/images/people` and edit the yaml in `data/people.yaml`
- To add or edit a **tool**, first upload any files you want downloadable to the `assets` folder. Then edit the yaml in `data/tools.yaml`. The complete yaml options available are:

```yaml	
  name: name of the tool
  docs: if an R package, link to online pkgdown docs
  gh_repo: Github repo name (excluding org; all tools should live in the CAPTURE-TB-HIV org)
  web: a web app if it exists
  excel: a downloadable Excel workbook if it exists
  doi: the DOI if it has one
  version: where shields.io should look for the package version. probably one of "r-package" or "package-json"
  paper: link to associated paper if it exists
  description: description of the tool
```
- To add or edit an output other than a tool, first upload any files that you want to make downloadable to the `assets` folder, then edit the yaml in `data/outputs.yaml`, adding the item to the list of **guidance**, **presentations**, or **papers**.