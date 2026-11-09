# My Zootopia — Animal Data Page Generator

A small Python project that reads animal records from JSON and generates an HTML page from a template. It was created as a learning project and currently contains the data loader and page template foundations.

## Project files

- `animals_web_generator.py` — JSON data-loading helper.
- `animals_data.json` — animal records used as input.
- `animals_template.html` — HTML template with a placeholder for generated animal information.

## Requirements

- Python 3.8 or later

No third-party packages are required for the currently committed Python helper; it uses Python's built-in `json` module.

## Current status

The repository currently provides the data-loading helper and HTML template. A complete generation workflow that fills `__REPLACE_ANIMALS_INFO__` and writes the finished page is not yet included. The template also contains Less-style variable declarations, so those should be converted to standard CSS (or compiled from Less) for direct browser use.

## Getting started

Clone the repository and inspect the source files:

```bash
git clone https://github.com/NeemaCharl/My-Zootopia.git
cd My-Zootopia
python -c "from animals_web_generator import load_data; print(len(load_data('animals_data.json')))"
```

The example assumes the JSON file contains a top-level list. If the data structure changes, adjust the example accordingly.

## Next steps

- Implement HTML generation and output-file writing.
- Add validation for missing or malformed animal data.
- Add tests for loading records and rendering a page.
- Make the template responsive and use browser-valid CSS.

## License

No license is currently specified. Unless a license is added, reuse and redistribution are not granted by default.

---

Created by [NeemaCharl](https://github.com/NeemaCharl).
