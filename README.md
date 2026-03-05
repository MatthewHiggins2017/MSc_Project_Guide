# MSc Project Guide 

### Setting up

It is best to do this in a fresh conda environment which you can make with

```
mamba create -n mkdocs -c conda-forge mkdocs-material -y
```

Then on your computer clone the repository:

```
git clone https://github.com/xxx
```

Checkout the `dev` branch:

```
git checkout dev
```

Activate the conda environment

```
conda activate mkdocs-material
```

Then go into the folder and run mkdocs serve

```
mkdocs serve
```

### Adding new tutorials

If you need add a new tutorial just create a new markdown file in `docs/<subdirectory>`. If you are running mkdocs serve your changes will automatically force the browser to refresh.

Adding the tutorial to the menu is done in `mkdocs.yml` under the `nav` section. Which has the folliwing format:

```yaml
nav:
  - Home: 
    - index.md
    - connecting-github.md
```

#### Images

All images can be placed using the following notation

```
![mapping_1](../img/Mapping_1.jpg)
```

