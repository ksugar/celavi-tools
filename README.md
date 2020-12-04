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
pip install -U .
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

## Notes

### branch lenghts mode

Please specify the `absolute` mode for importing into CeLaVi.

### did format

The `did` for CeLaVi is generated as "ID_`ID` _`name`" using the `Spot` attribute in the MaMuT xml.

```xml
<Spot ID="100" name="abc" POSITION_X="1.0" POSITION_Y="1.0" POSITION_Z="1.0" FRAME="0" POSITION_T="0.0" QUALITY="-1.0" VISIBILITY="1" RADIUS="1.0" />
<Spot ID="101" name="abc" POSITION_X="2.0" POSITION_Y="2.0" POSITION_Z="2.0" FRAME="1" POSITION_T="1.0" QUALITY="-1.0" VISIBILITY="1" RADIUS="1.0" />
```

will generate the CeLaVi nodes with the following `did`s.

```
ID_100_abc
ID_101_abc
```

## License

Apache-2.0 License.

## Acknowledgements
* Irepan Salvador-Martinez