# Serious Games Survey: Data Processing and Segmentation

A modular Python command-line tool that loads, cleans, segments, analyzes and exports survey data evaluating the features of serious video games.

**Team project, Tecnológico de Monterrey:** Ángel Nicolás Landa Tapia, Ximena Paola Pérez Sánchez, Axel Yael Rodríguez Romero, Emilio Estrada Pérez, Juan Diego Rodríguez Espinoza.
<!-- Optional: add a line with your own contributions, e.g. **My contributions:** ... -->

## Features

1. Loads survey responses from an `.xlsx` file.
2. Filters responses by informed consent and prior video game experience.
3. Segments respondents interactively by gender and age range.
4. Builds separate datasets for feature importance and feature ratings.
5. Computes means and standard deviations of the evaluated features.
6. Exports the results to a multi-sheet Excel file.

## Project structure

```
.
├── main.py           # Entry point
├── clean.py          # Data loading and cleaning
├── cli.py            # Interactive console interface for segmentation
├── segment.py        # Segmentation by gender and age range
├── group.py          # Builds the importance and ratings DataFrames
├── analyze.py        # Mean and standard deviation analysis
├── export.py         # Export of results to Excel
└── requirements.txt
```

The survey data is excluded from the repository for privacy.

## Getting started

Requires Python 3.9 or later.

```bash
pip install -r requirements.txt
python main.py
```

Place the input file `respuesta_de_encuestas.xlsx` in the project directory, or pass its path on the command line.

## Output

The tool generates `resultados_encuesta.xlsx` with three sheets:

- **Full Data:** all selected columns after cleaning and segmentation.
- **Importance:** importance ratings of the evaluated features.
- **Ratings:** feature ratings and the overall game rating.

## License

Developed for academic purposes.
