# Iterative Closest Point (ICP) Algorithm Implementation

This repository contains a Python implementation of the Iterative Closest Point (ICP) algorithm, a fundamental technique used in 3D point cloud registration. The algorithm is demonstrated in a step-by-step Jupyter Notebook.

This project is a demonstration of core concepts in computational imaging and computer vision, specifically for solving geometric alignment problems.

## ℹ️ About the Project

The ICP algorithm is used to find the optimal rigid transformation (rotation and translation) that aligns a "source" point cloud to a "target" point cloud.  
Data is here: https://drive.google.com/drive/folders/1ayBozT1QAVTLbs1M8UbZXeXOMtDUToyl?usp=drive_link

This implementation in `ICP_Algorithm.ipynb` demonstrates the complete process:
1.  **Data Loading:** Reading two point clouds (`scene1_perspective1.ply` and `scene1_perspective2.ply`) using Open3D.
2.  **Downsampling:** Reducing the number of points via voxel-based downsampling for faster computation.
3.  **Association:** Finding the closest corresponding points between the two clouds using a KD-Tree (`scipy.spatial.cKDTree`).
4.  **Transformation Calculation:** Computing the optimal rotation and translation using Singular Value Decomposition (SVD).
5.  **Iteration:** Applying the transformation and repeating the process until the alignment error (RMSE) converges below a threshold.

## 🛠️ Built With

This algorithm is implemented using standard Python scientific computing libraries:
* [Python](https://www.python.org/)
* [NumPy](https://numpy.org/) - For all matrix operations and transformations.
* [SciPy](https://scipy.org/) - For KD-Tree nearest neighbor search.
* [Open3D](http://www.open3d.org/) - For reading and visualizing point clouds.
* [Matplotlib](https://matplotlib.org/) - For 3D visualization of the alignment.
* [Jupyter Notebook](https://jupyter.org/) - For interactive demonstration and visualization.

## 🚀 Getting Started

To run this simulation on your local machine, follow these steps.

### Prerequisites

Ensure you have Python and pip installed.

### Installation

1.  Clone the repository:
    ```sh
    git clone https://github.com/Didemld/ICP-Algorithm.git
    ```
2.  Navigate to the project directory:
    ```sh
    cd ICP-Algorithm
    ```
3.  Install the required Python packages:
    ```sh
    pip install numpy scipy matplotlib open3d jupyterlab
    ```
4.  Start Jupyter Lab and open the notebook:
    ```sh
    jupyter lab ICP_Algorithm.ipynb
    ```

## 📊 Demonstration (Placeholder)

<img width="792" height="812" alt="image" src="https://github.com/user-attachments/assets/a5356a06-e8d4-4ee4-ac67-b177e1a79072" />
<img width="792" height="790" alt="image" src="https://github.com/user-attachments/assets/aeae6bf7-7da0-4dea-82b8-0a273135de0a" />

[Image/GIF of the algorithm in action: showing the initial misaligned point clouds and the final registered result]

## 👤 Contact

**Didem Doğan Başkaya**  
* **LinkedIn:** [`in/didemdoganbaskaya`](https://www.linkedin.com/in/didemdoganbaskaya)  
* **GitHub:** [`Didemld`](https://github.com/Didemld)
