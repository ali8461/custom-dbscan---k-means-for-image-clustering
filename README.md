
---

# 🧠 Custom DBSCAN & K-Means for Image Clustering

A **Data Mining** project that implements **custom versions of DBSCAN and K-Means** clustering algorithms from scratch, optimized for clustering pixels in images. This project demonstrates the application of unsupervised learning for tasks like **image segmentation**, **anomaly detection**, and **pattern recognition**.

---

## 📌 Project Highlights

* ✅ **Custom DBSCAN**: Improved noise handling and adaptive neighborhood detection for better performance on high-dimensional pixel data.
* ✅ **Enhanced K-Means**: Customized initialization and Euclidean distance handling tailored to image features.
* ✅ **Feature Engineering**: Efficient reshaping and clustering of RGB pixel values.
* ✅ **Scalability**: Designed to work efficiently on medium to large image datasets.
* ✅ **Applications**: Image segmentation, unsupervised image clustering, and noise-based anomaly detection.

---

## 📂 Project Structure

```
📁 image_clustering_project/
├── clustering_algorithm.py       # Custom DBSCAN and K-Means implementations
├── clustering_task.ipynb         # Notebook to run clustering on images
├── giraffe.png                   # Sample image used for clustering
├── kmeans_output.jpg             # Output image clustered by K-Means
├── dbscan_output.jpg             # Output image clustered by DBSCAN
└── README.md                     # You're here!
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/image-clustering-project.git
cd image-clustering-project
```

### 2. Install Dependencies

This project uses only a few standard Python libraries:

```bash
pip install numpy matplotlib opencv-python scikit-learn
```

> ✅ No deep learning or external ML libraries used — fully custom implementations.

---

## 🖼️ Running the Project

Open the Jupyter notebook and run each cell step-by-step:

```bash
jupyter notebook clustering_task.ipynb
```

### Customize Image

You can replace the `giraffe.png` with any other image:

```python
image_path = 'your_image.jpg'
```

### Adjust Parameters

In the notebook, you can modify these for experimentation:

```python
# K-Means
k = 4

# DBSCAN
eps = 5
min_pts = 10
```

---

## 📊 Results

Clustering results are visualized side-by-side:

* **Original Image**
* **K-Means Segmented Image**
* **DBSCAN Segmented Image**

Each pixel is colored based on its assigned cluster's average RGB value.

---

## 🛠️ Implementation Details

### K-Means:

* Random center initialization using `random_state`.
* Iterative assignment and update steps.
* Convergence check on centroid stability.

### DBSCAN:

* Euclidean distance-based neighborhood expansion.
* Custom labeling logic for visited, core, and noise points.
* Dynamic cluster formation without needing a predefined number of clusters.

---

## 📈 Sample Output

| Original                       | K-Means                      | DBSCAN                       |
| ------------------------------ | ---------------------------- | ---------------------------- |
| ![original](kmeans_output.jpg) | ![kmeans](kmeans_output.jpg) | ![dbscan](dbscan_output.jpg) |

---

## 💡 Use Cases

* **Image Segmentation** (e.g., medical, satellite images)
* **Pattern Recognition**
* **Noise-based Anomaly Detection**
* **Unsupervised Learning Research**

---

## 📜 License

This project is part of an academic data mining assignment. If reused, please give credit to the author.

---

## 🙋‍♂️ Author

**Muhammad Ali**
*Data Mining Enthusiast | AI Explorer*


---

