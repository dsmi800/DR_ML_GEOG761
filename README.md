# GEOG 761 Project - Applying machine learning to satellite imagery for rapid disaster response following the 2023 Morocco earthquake

## Background:
- This code can be applied to any disaster released under the Maxar Open Data Program

## Data
Maxar Open Data Program - imagery of Morocco Earthquake https://www.maxar.com/open-data/morocco-earthquake-september-2023

## Models used
Building damage assessment used the ChangeOS model https://github.com/Z-Zheng/ChangeOS?search=1
- This model was trained on xBD data

Road damage assessment used the CRESI model https://github.com/avanetten/cresi

## Process to run the code
1. Run <code>DownloadMoroccoData.ipynb</code> to download the Morroco Earthquake Data
2. Run the <code>DataDirectorySetUp.ipynb</code> to format the data for use in later scripts
3. Run the <code>MosaicAndClip.ipynb</code> script to mosaic the pre- and post- disaster imagery, then clip pre-disaster imagery so that it covers areas that the post-disaster imagery covers
4. Run the <code>BDA_tiled.ipynb</code> script to run building damage detection on post-disaster imagery and visualise results
5. Run the road damage detection script (TBC)
