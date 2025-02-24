# 🛰️ Water Body Detection Using Remote Sensing

This repository contains an Image Mining project focused on water body detection using remote sensing data. The study explores different sensing technologies, a multi-modal approach combining optical and SAR data, and methods such as Normalized Difference Water Index (NDWI) and deep learning-based segmentation for accurate water detection.

## 📌 Overview

🌍 Why Remote Sensing for Water Detection?

Water bodies play a crucial role in environmental monitoring, disaster response, and climate studies. Detecting them from satellite imagery enables large-scale analysis without the need for in-situ measurements.

🔍 Key Topics Covered:
	•	Evaluation of different sensor types (optical, SAR, LiDAR, SAR altimeters) for water body detection.
	•	Multi-modal sensor fusion: Combining Sentinel-1 (SAR) and Sentinel-2 (optical) to improve detection across different environmental conditions.
	•	Open vs. commercial satellite data: Choosing publicly available high-resolution (HR) imagery over very-high-resolution (VHR) commercial datasets.
	•	NDWI for non-learning-based detection: Extracting water regions based on spectral indices.
	•	Deep learning segmentation: Testing a U-Net model on a public remote sensing dataset.

## 🚀 Prerequisites

Ensure you have Python 3.8+ installed. Clone the repository:

git clone https://github.com/lmcastanedame/ImageMining_RemoteSensing.git
cd ImageMining_RemoteSensing

## 🏗 Usage

1️⃣ Sensor Evaluation & Data Selection

The study evaluates different sensors for water detection:
	•	Sentinel-2 (Optical): High-resolution multispectral imagery for NDWI computation.
	•	Sentinel-1 (SAR): Weather-independent imaging to complement optical data.
	•	LiDAR & SAR altimeters: Specialized sensors considered for future work.

2️⃣ NDWI-Based Water Detection (Non-Learning Approach)

Run the script to compute NDWI and generate a binary water mask:

- Formula: NDWI = (Green - NIR) / (Green + NIR)
- Bands used: Sentinel-2 Band 3 (Green) & Band 8 (NIR)
- Output: Binary water mask (highlights detected water bodies)

## 📚 References
- McFeeters, S.K., “The use of the Normalized Difference Water Index (NDWI) in the delineation of open water features,” International Journal of Remote Sensing, 1996.
- Otsu, N., “A Threshold Selection Method from Gray-Level Histograms,” IEEE Transactions on Systems, Man, and Cybernetics, 1979.
