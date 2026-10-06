```markdown
# Sensor Fusion and Point Cloud Processing

A computer vision project demonstrating LiDAR-Camera sensor fusion and point cloud processing using the NuScenes autonomous driving dataset.

## Features

Sensor Fusion

- LiDAR point cloud loading from NuScenes
- Coordinate system transformations:
  - LiDAR → Ego Vehicle
  - Ego → Global
  - Global → Camera Ego
  - Camera Ego → Camera
- LiDAR point projection onto camera images
- Depth-based color visualization
- Camera-LiDAR fusion visualization

Point Cloud Processing

- LiDAR point cloud parsing
- Global coordinate transformation
- Voxel downsampling
- Statistical outlier removal
- Ground plane extraction
- DBSCAN clustering
- Top-view visualization of ground and object points

## Project Structure

Point_Cloud/
├── results/                     # Point cloud processing outputs
├── fusion_results/              # Fusion output images
├── Point_Cloud.ipynb            # Main Jupyter notebook
└── requirements.txt             # Python dependencies

## Installation

```bash
git clone https://github.com/f-naderi/Point_Cloud.git
cd Point_Cloud
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```


## Requirements

* Python 3.10+
* Matplotlib
* NumPy
* Open3D
* Scikit-Learn
* Pillow
* PyQuaternion
* NuScenes Devkit
* Jupyter Notebook


## References

- NuScenes Dataset — Caesar et al., 2020
- Open3D — Zhou et al., 2018
- DBSCAN — Ester et al., 1996
- RANSAC — Fischler & Bolles, 1981
- Sensor Fusion for Autonomous Driving

```
