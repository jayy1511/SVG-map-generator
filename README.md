# SVG Map Generator

SVG Map Generator is a Python tool that converts GeoJSON data into SVG maps, providing a simple and customizable way to visualize geographic information.

## Features

- Converts GeoJSON files into SVG maps
- Supports various geometric objects such as points, lines, polygons, etc.
- Customizable styling for different map elements
- Simple command-line interface for rendering maps in batch

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/SVG-map-generator.git
    ```

2. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Ensure you have your GeoJSON files ready.

2. Run the `main.py` script, passing the directory containing GeoJSON files as an argument:

    ```bash
    python main.py /path/to/geojson/files
    ```

    This will convert each GeoJSON file into an SVG map and save it in the same directory with the same name but with the `.svg` extension.

## Customization

You can customize the styling of map elements and the SVG template by modifying the code in the `map-template.svg` file and the classes in the `MapElement` module.

## Example

```python
# Example GeoJSON file: example.json

{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Point",
        "coordinates": [0, 0]
      },
      "properties": {
        "id": "example_point"
      }
    }
  ]
}
