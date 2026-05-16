# persistent-bare-soil-exposure-indicator
Google Earth Engine workflows, validation tables, and reproducibility materials for Sentinel-2 persistent bare-soil exposure indicator development in temperate agricultural landscapes (Minsk Region, Belarus, 2020–2025).


This repository contains the Google Earth Engine publication workflow and supporting materials for the manuscript:

“Persistent Bare-Soil Exposure as a Sentinel-2 Ecological Indicator of Recurrent Land-Surface Pressure in Temperate Agricultural Landscapes”.

The workflow includes Sentinel-2 preprocessing, scene-level bare-soil detection, annual bare_frac construction, observation-density metadata, persistence-threshold sensitivity analysis, annual hotspot area summaries, six-year recurrence mapping, and candidate reference-point generation.

Some input assets used in the manuscript, including the study-area boundary, administrative boundaries, soil-landscape stratification layer, and interpreted validation points, are not redistributed in this repository because they are derived from institutional or restricted datasets. Users should replace the placeholder asset paths with equivalent local datasets before running the scripts.

Workflow dependency:
1. Run the annual bare_frac export module for each year from 2020 to 2025.
2. The annual products generated in Step 1 are then used for persistence sensitivity, annual area summaries, and recurrence mapping.
3. Candidate reference points require manual interpretation before use in accuracy assessment.
