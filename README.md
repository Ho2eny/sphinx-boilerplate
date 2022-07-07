# sphinx-boilerplate
Boilerplate that deploys reStructuredText docs to Github Page 

## Build the docs

**Install Sphinx and Theme**

```shell
pip install -r requirements.txt
```

**Building the docs**

In the `docs/` folder

```shell
make html
```

If you want to building each time a file is changed

```shell
sphinx-autobuild . _build/html
```

## Deploys docs with Github Pages

When you push some `.rst` documents to `master`, **Github Action** builds sphinx and deploys static html to `gh-pages` branch.

You can publish the `gh-pages` branch on **Github Pages**

Set the **Github Pages** source to `gh-pages` `/(root)` in the repository **Settings**