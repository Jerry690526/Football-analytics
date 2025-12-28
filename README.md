# Football Analytics & Network Science Portfolio

[![License: MIT](https://img.shields.io/badge/License-MIT-lightgrey.svg)](#license)
[![Status](https://img.shields.io/badge/status-active-brightgreen.svg)]()

A collection of projects applying Complex Systems, Network Science, and Statistical Modeling to football (soccer) data. The portfolio highlights reproducible analyses, visualizations and modeling techniques used to extract tactical and performance insights from event and tracking data.

## Featured Projects (default)
### 1. Football Spatial & Statistical Modeling
- Description: Pitch-control models to evaluate space occupation and derive zone-level performance metrics from tracking data.
- Technical details: Modeled probability of a team maintaining possession in pitch zones using kinematic features (velocity, acceleration) and player positions.
- Tools: Scikit-learn, Pandas, mplsoccer
- Files: notebooks/pitch_control_model.ipynb

### 2. Passing Flows as Vector Fields
- Description: Represent pass collections as continuous vector fields to quantify directionality and intensity of ball movement; identify dominant attacking lanes.
- Impact: Provides a continuous, spatially-resolved view of team momentum beyond discrete pass events.
- Tools: NumPy, SciPy, matplotlib, mplsoccer
- Files: notebooks/passing_vector_fields.ipynb

## Other Projects
### World Cup Pass Network Analysis (Argentina 2022)
- Description: Network analysis mapping player connectivity to identify tactical pivots and information flow within the team.
- Key methods: centrality measures, shortest-path and path-length metrics, community detection.
- Tools: Python, NetworkX, statsbombpy, Matplotlib
- Key findings: Quantified player influence on transitions and identified high-centrality pivots that coordinated attacking phases.
- Files & repo: See [Jerry690526/football-analytics](https://github.com/Jerry690526/football-analytics) (notebooks/worldcup_pass_networks.ipynb)

## Technical Toolkit
- Modeling: Network Science, Pitch Control, Expected Goals (xG), Expected Threat (xT)
- Languages: Python (Pandas, NumPy, Scikit-learn), R, MATLAB, C++
- Visualization: Matplotlib, mplsoccer, LaTeX, Xmgrace

## Reproducibility / Getting started

1. Clone
   - git clone https://github.com/<owner>/<repo>.git

2. Create environment (conda recommended)
   - conda create -n football-analytics python=3.10
   - conda activate football-analytics
   - pip install -r requirements.txt

3. Requirements (example)
   - pandas, numpy, networkx, statsbombpy, scikit-learn, matplotlib, mplsoccer, jupyterlab

4. Data
   - Event data: StatsBomb or other event datasets (see `data/README.md`).
   - Tracking data: Use provided sample files in `data/tracking_sample/` or obtain from providers respecting licensing terms.
   - Note: Some notebooks expect StatsBomb format (statsbombpy can fetch public competitions). Sensitive/proprietary datasets are not included.


