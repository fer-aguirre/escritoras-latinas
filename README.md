### [Español](README-ES.md)
---

# Latin American Women Writers

This repository was developed for the code and data behind the story [Una constelación de escritoras latinoamericanas (nacidas en el siglo XX).](https://datacritica.org/portfolio/constelaciones-de-escritoras-latinoamericanas-nacidas-en-el-siglo-xx/)

The analysis uses web scrapping of Wikipedia entries for Latin American women writers and network graph visualization in order to create a [web application](http://escritoraslatam.datacritica.org/).

---

## Directory Structure

```
├── app.py                              # Streamlit app file
├── assets                              # Resources for the project
│   ├── datacritica
│   ├── imgs
│   ├── imgs_processed
│   ├── mosaics
│   ├── targets
│   └── targets_processed
├── data                                # Categorized data 
│   ├── processed                       # Cleaned data
│   │   ├── escritoras_wiki.csv
│   │   └── escritores_destacados.csv
│   └── raw                             # Original data
│       └── escritoras.csv
├── Dockerfile                          # Commands to build a docker image
├── docs                                # Explanatory materials
│   ├── data-dictionary.md              # Information about the data
│   └── references                      # Papers, manuals, articles, etc.
├── escritoras_latinas                  # Python package
│   ├── data                            # Functions to manipulate data
│   │   ├── analyze.py                  # Module to analyze data
│   │   ├── export.py                   # Module to save exports
│   │   ├── load.py                     # Module to load data and paths
│   │   └── process.py                  # Module to process data
│   └── utils                           # Functions to make common patterns
│       └── paths.py                    # Module to generate relative paths
├── LICENSE                             # Project license
├── notebooks                           # Jupyter notebooks
│   ├── 0.0-scrapping-text.ipynb
│   ├── 0.1-scrapping-text.ipynb
│   ├── 0.2-scrapping-images.ipynb
│   ├── 1.0-annotate-data.ipynb
│   ├── 1.1-process-images.ipynb
│   ├── 2.0-visualize-network.ipynb
│   └── 2.1-visualize-donut-chart.ipynb
├── outputs                             # Exports generated by notebooks
│   ├── figures                         # Generated graphics, maps, etc.
│   │   └── index.html
|   ├── networks                        # Generated graph network
│   │   └── index.html
│   └── tables                          # Generated pivot tables
│   ├── LICENSE
│   ├── photomosaics
│   │   ├── photomosaics.py
│   │   ├── run.py
│   │   └── scrape.py
│   ├── README.md
│   └── requirements.txt
├── Pipfile                             # Project dependencies
├── Pipfile.lock                        # Specific versions of packages on Pipfile
├── README.md                           # Top-level README for this project
├── README-ES.md                        # README in Spanish
├── requirements.txt                    # Project dependencies
├── setup.py                            # Import project as a python module
└── style.css                           # Styles for streamlit app
```
---

## License

This project is released under [MIT License](/LICENSE).

---

This repository was generated with [cookiecutter](https://github.com/cookiecutter/cookiecutter) using a [data-journalism](https://github.com/DataCritica/cookiecutter-data-journalism) template for python.