# London Crime Hotspot Stability Analysis

## Overview
This project examines whether London’s crime hotspots stay in the same places over time. It compares hotspot patterns across different time windows (the last 3 months versus the last 12 months) and across different crime measures (total crime versus violence against the person). The project was developed as a short analytical brief combining spatial analysis, statistics, and visual communication.

## Research question
Do London’s crime hotspots stay in the same places over time, or does the answer change depending on the time window and crime type used?

## Tools used
- Python
- GeoPandas
- spatial statistics
- data visualisation
- London LSOA-level crime, population, and boundary data

## What I analysed
- Crime rates per 1,000 residents across 4,988 London LSOAs
- Hotspot stability across 3-month and 12-month time windows
- Differences between total crime and violence-against-the-person patterns
- Rank stability using Spearman’s correlation
- Spatial clustering using Global Moran’s I and Local Moran’s I (LISA)

## Method
To compare hotspot stability, I first calculated crime rates per 1,000 residents for each London LSOA. I then identified hotspots using a top 20% threshold and compared results across:
- total crime and violence against the person
- 3-month and 12-month time windows

I used two main measures of stability:
- hotspot overlap
- Spearman’s rank correlation

I also used Global Moran’s I and Local Moran’s I (LISA) to examine whether hotspot patterns were spatially clustered.

## Key findings
- Total crime hotspots are mostly stable over time. Around 87.4% of 3-month total-crime hotspots also remain hotspots in the 12-month view.
- Violence hotspots are less stable. Around 74.7% of 3-month violence hotspots also remain hotspots in the 12-month view.
- The picture of “crime hotspots” depends on what is measured. Different crime types can produce different hotspot maps.
- Hotspots often appear in clusters rather than isolated single areas, supported by positive spatial autocorrelation (Global Moran’s I = 0.514, p = 0.001).

## Outputs
This repository contains:
- hotspot maps
- distribution charts
- scatterplots
- spatial clustering diagnostics
- a short written analytical brief

## Why this project matters
This project shows that hotspot stability is not a simple yes-or-no question. The answer depends on both the time window and the crime indicator used. This matters for how crime data is interpreted and communicated, especially when results are presented to broader audiences or used to support place-based decision-making.

## Files in this repository
- `25109433.pdf` – project brief / final write-up
- `figures/` – maps, charts, and visual outputs
- `notebooks/` or `scripts/` – analysis workflow (if included)

## Author
Hanyun Hu
