# *pynanovna*
![PyPI - Version](https://img.shields.io/pypi/v/pynanovna)
![PyPI - Downloads](https://img.shields.io/pypi/dm/pynanovna)
![PyPI - License](https://img.shields.io/pypi/l/pynanovna)
![GitHub Repo stars](https://img.shields.io/github/stars/PICC-Group/pynanovna)


This is a python module for using a NanoVNA.


## 🌟 Features
    ✅ Supporting almost all NanoVNAs.
    🔄 Streaming of s11 and s21 data.
    📶 Run single sweeps.
    🛠️ Calibrate your NanoVNA.
    📊 Interactive, real-time plotting of data.
    📁 Recording to CSV files.


## 🛠️ Installation
Install with `pip install pynanovna`.

## 🚀 Example
```
import pynanovna

vna = pynanovna.VNA()

vna.set_sweep(2.0e9, 2.6e9, 101)

stream = vna.stream()
for s11, s21, frequencies in stream:
    print(s11, s21, frequencies)
```

See `src/pynanovna/example.py` for a more detailed example on some use cases of the project.

See `src/pynanovna/calibration_helper.py` for details on how to calibrate you NanoVNA.

## 📚 API Reference
API Reference is available at [pynanovna.readthedocs.io](https://pynanovna.readthedocs.io/en/latest)

## 📖 Cite This Library

If you use *pynanovna* in your research or project, please cite it as follows:

**BibTeX**
```bibtex
@software{pynanovna,
  author = {PICC-Group, Teo Bergkvist},
  title = {pynanovna: A Python Module for NanoVNA},
  year = {2024},
  url = {https://github.com/PICC-Group/pynanovna},
  version = {1.0.0},
}
```
## 📜 Licence
*pynanovna* is under GNU General Public License.

## 🕰️ History
Originally this was the fork [nanovna-saver-headless](https://github.com/PICC-Group/nanovna-saver-headless) from [nanovna-saver](https://github.com/NanoVNA-Saver/nanovna-saver) but when that project no longer shared much code with the original we decided to create a new project.

# ⭐️ If you find *pynanovna* useful, please support us by starring the repository ⭐️
