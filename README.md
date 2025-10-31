# LULC Streamlit App

This project is an interactive Land Use Land Cover (LULC) digitization tool built using Streamlit. It allows users to select LULC classes, draw features on a map, and capture data for analysis.

## Project Structure

```
lulc-streamlit-app
├── .gitignore
├── .streamlit
│   └── config.toml
├── .devcontainer
│   ├── devcontainer.json
│   └── Dockerfile
├── data
│   ├── lc_pedamaran.csv
│   ├── aoi_pedam.shp
│   ├── aoi_pedam.shx
│   ├── aoi_pedam.dbf
│   ├── Pedamaran_sample.shp
│   ├── Pedamaran_sample.shx
│   └── Pedamaran_sample.dbf
├── src
│   └── interactive_sampling_tool.py
├── streamlit_app.py
├── requirements.txt
├── setup.cfg
├── pytest.ini
└── README.md
```

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd lulc-streamlit-app
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. (Optional) If using a development container, open the project in a compatible IDE and build the container.

## Usage

To run the Streamlit application, execute the following command:
```
streamlit run streamlit_app.py
```

Once the application is running, you can interact with the map to digitize LULC features by selecting classes and drawing points or polygons.

## Data

- The `data/lc_pedamaran.csv` file contains the LULC classes with their respective IDs and color palettes.
- The AOI shapefile (`data/aoi_pedam.shp`, `data/aoi_pedam.shx`, `data/aoi_pedam.dbf`) defines the area of interest for digitization.
- The optional training data shapefile (`data/Pedamaran_sample.shp`, `data/Pedamaran_sample.shx`, `data/Pedamaran_sample.dbf`) can be loaded to utilize existing training data.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.