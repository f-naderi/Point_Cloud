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

- Caesar, H., Bankiti, V., Lang, A. H., Vora, S., Liong, V. E., Xu, Q., ... & Beijbom, O. (2020, June). nuscenes: A multimodal dataset for autonomous driving. In 2020 IEEE/CVF conference on computer vision and pattern recognition (CVPR) (pp. 11618-11628). IEEE.
- Zhou, Q. Y., Park, J., & Koltun, V. (2018). Open3D: A modern library for 3D data processing. arXiv preprint arXiv:1801.09847.
- Ester, M., Kriegel, H. P., Sander, J., & Xu, X. (1996, August). A density-based algorithm for discovering clusters in large spatial databases with noise. In kdd (Vol. 96, No. 34, pp. 226-231).
- Bolles, R. C., & Fischler, M. A. (1981, August). A ransac-based approach to model fitting and its application to finding cylinders in range data. In Ijcai (Vol. 1981, pp. 637-643).
- Merangolo, M. F. (2025). Sensor Fusion for Autonomous Driving (Doctoral dissertation, Politecnico di Torino).

```
