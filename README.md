Landfill Leachate Generation & Hydrological Sensitivity Analysis (HELP Model)

A complete computational study exploring post-closure landfill hydrology, using the HELP model, parametric sensitivity analysis, and layer-wise water storage modeling for the Matuail Sanitary Landfill (Dhaka, Bangladesh).

📌 Overview

This repository contains all scripts, data, visualizations, and results used to:

Model leachate generation over a 30-year post-closure period

Evaluate effects of:

Leaf Area Index (LAI)

Evaporative Zone Depth (EZD)

Cover soil permeability

Cover thickness

Compacted Clay Liner (CCL) permeability

Municipal Solid Waste (MSW) permeability

Generate heatmaps, layer-wise water storage plots, and sensitivity analyses

Preprocess multi-year NASA POWER, NOAA, and NSRDB weather datasets

Produce cross-sectional diagrams of the landfill system

Run full centimeter-scale and volumetric water storage models

📂 Repository Structure
data/
    weather/                # Cleaned weather data
    model_raw/              # Raw HELP model outputs
    layer_storage_raw/      # LAI, EZD, CCL, MSW water storage raw data

src/
    preprocessing/          # Weather + workbook processing
    graphing/               # Cross-sections & scale-break figures
    parameters/             # LAI, EZD, Cover, CCL, MSW scripts
    layer_water_storage/    # cm-scale + volumetric models

results/
    plots/
    heatmaps/
    sensitivity/
    layer_water_storage/
    reports/

notebooks/                  # Optional Jupyter notebooks

🧠 Key Features

HELP model automation

Layer-by-layer hydrological response visualization

Sensitivity radar charts

Cross-section engineering drawings

Heatmap generation (annual & peak responses)

Massive dataset processing (1991–2023)

▶ How to Run

Install dependencies:

pip install -r requirements.txt


Run any parameter analysis:

python src/parameters/LAI/LAI_graph.py


Run layer water storage model:

python src/layer_water_storage/centi/main_script_cm_fixed2.py

✨ Authorship

Asif Mahmoud
Bangladesh University of Engineering and Technology (BUET)
Department of Civil Engineering — Environmental Engineering