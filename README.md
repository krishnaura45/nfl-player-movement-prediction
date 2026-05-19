# NFL - Big Data Bowl 2026 ~ `Actual 85th Place Solution`
> Predicting NFL player movement trajectories during live pass plays using geometric deep learning and neural network inference pipelines<br>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Graph Neural Network](https://img.shields.io/badge/Graph-Neural%20Networks-blueviolet?style=for-the-badge)
![RMSE Optimized](https://img.shields.io/badge/Optimized--for-RMSE-yellowgreen?style=for-the-badge)
![Best Score](https://img.shields.io/badge/Best%20Score-0.541-2ECC71?style=for-the-badge)
![Rank](https://img.shields.io/badge/Rank-139%20of%201899-brightgreen?style=for-the-badge)
![Solo](https://img.shields.io/badge/Submission-Solo-orange?style=for-the-badge)

### **Duration**: 
- First Submission ~ Sep 28, 2025
- Last Submission ~ Dec 17, 2026

---


## File Structure

```bash
nfl-player-movement-prediction/
│
├── INFO.md
├── README.md
├── inference-dynamic-specs-nn.ipynb
├── inference-geometry-gnn.ipynb
│
├── output/
│   └── submission.parquet
```

---

## Problem Statement

The objective of the [NFL - Big Data Bowl 2026 - Prediction] competition was to predict player movement trajectories during the frames after a quarterback releases the football.

Using NFL Next Gen Stats tracking data prior to the throw, along with contextual information such as targeted receiver and projected ball landing location, participants were required to forecast future player positions frame-by-frame while the ball remained in the air.

This challenge emphasized:

- Dynamic multi-agent interaction modeling
- Spatio-temporal trajectory forecasting
- Real-time inference constraints
- Player geometry and movement understanding

Submissions were evaluated using **Root Mean Squared Error (RMSE)** between predicted and actual `(x, y)` player coordinates over future frames. Lower RMSE indicated better forecasting performance.

---

## Approach

Main Notebook: [`inference-geometry-gnn.ipynb`](./inference-geometry-gnn.ipynb)

Key steps implemented in the final solution:

### 1. Geometry-Aware Player Representation
- Modeled player interactions using spatial relationships and geometric positioning.
- Leveraged relative movement dynamics between offensive and defensive players.

### 2. Graph Neural Network Based Modeling
- Constructed graph-style representations of player movement states.
- Captured interaction-aware dependencies between nearby players during pass plays.

### 3. Spatio-Temporal Feature Processing
- Incorporated positional movement signals from tracking frames before ball release.
- Utilized contextual movement structure to improve downstream trajectory prediction.

### 4. Iterative Experimental Modeling
- Explored multiple inference strategies and architectures during experimentation.
- Maintained alternative approach notebook:
  - [`inference-dynamic-specs-nn.ipynb`](./inference-dynamic-specs-nn.ipynb)

### 5. Submission
- Produced final predictions in parquet format compatible with Kaggle evaluation API.
- Stored final outputs inside:
  - `output/submission.parquet`

---

## Competition Results

### Public/Private LB Scores (over 15+ submissions)
- 0.88814
- 0.69436
- 0.62422
- 0.61121
- 0.58025
- 0.56768
- 0.54095

### Placement
- Ranked `139` out of `1899` teams
- Competed as a **solo participant**

---

## References

- Competition Data: [NFL 2026 - Prediction](https://www.kaggle.com/competitions/nfl-big-data-bowl-2026-prediction/data)
- Other Datasets:
  - [NFL - GRU + GNN Models](https://www.kaggle.com/datasets/pankajiitr/nfl-bdb-2026)
  - [NFL - LSTM Models](https://www.kaggle.com/datasets/llkh0a/nfl-big-data-bowl-2026-public)
- Other Helpful Sources:
  - [NFL Big Data Bowl](https://operations.nfl.com/gameday/analytics/big-data-bowl/)
  - [NFL Next Gen Stats](https://nextgenstats.nfl.com/)

---

## Tech Stack

- **Language**: Python 
- `pandas`, `numpy`
- `PyTorch`
- Graph NN utilities
- Kaggle Evaluation API utilities
- Kaggle Notebooks and GPU-based experimentation

---

📌 *This project demonstrates the application of geometric deep learning and spatio-temporal modeling for real-world player trajectory forecasting in professional sports analytics.*
