# CeLaVi tools

## Available tools

* `mamut_to_celavi`: A python executable for converting a MaMuT xml to CeLaVi json/csv.

## Getting Started

### Prerequisites

Python3 + pip

### Clone

```bash
git clone https://github.com/ksugar/celavi-tools.git
```

### Installation

Run the following command at the root directory of thie repository.

```bash
pip install .
```

## Usage

```bash
mamut_to_celavi mamut.xml tree.json 3D_cells.csv

# usage: mamut_to_celavi [-h] input json csv
#
# positional arguments:
#   input       MaMuT xml file to convert
#   json        JSON file to output trees
#   csv         CSV file to output cells
#
# optional arguments:
#   -h, --help  show this help message and exit
```

## License

Apache-2.0 License.

## Acknowledgements
* Irepan Salvador-Martinez