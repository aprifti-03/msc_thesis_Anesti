# MSc Thesis: Secular Resonance in Protoplanetary Disc Systems

This repository contains Python simulations and plotting materials for an MSc thesis studying secular precession resonances and the evolution of misalignment between circumstellar discs, a companion orbit, and circumbinary discs. The model implementations are based on Owen & Lai (2017), *MNRAS*, 469, 2834.

## Repository contents

- **`Accretion/`** — accreting-companion simulations and generated figures/animations, organized into folders for systems including HD 135344B, HD 142527, HD 143006, V1098 Sco, and Wray 15-788. The main implementation is `accretionmethod.py`.
- **`parameter_study/`** — parameter sweeps and heatmap outputs. `parameterstudy.py` runs an accreting-scenario study over companion/disc parameters and plots final and maximum misalignment angles.
- **`Plot_recreation/`** — scripts and outputs for recreating selected accretion and migration plots. The migration model is implemented in `migrationmethod.py`.

The repository includes generated plots and other results alongside the Python source. Some data/output folders are system-specific; refer to the relevant script and folder when working with a particular system.

## Requirements

Python 3.9 or newer is recommended. The source imports:

- NumPy
- SciPy
- Matplotlib
- Pillow (needed to save GIF animations)

Install the dependencies with:

```bash
python -m pip install numpy scipy matplotlib pillow

python Accretion/accretionmethod.py

python parameter_study/parameterstudy.py

python Plot_recreation/migrationmethod.py
