
# Cloud Data Processing & Distributed ML Pipeline (AWS EMR + PySpark)

## Project Overview
This project focuses on designing a scalable cloud-based data processing pipeline for distributed computation and machine learning workflows.

The system demonstrates how large-scale datasets can be processed using AWS EMR and PySpark, with emphasis on **scalability, cost efficiency, and privacy-aware data handling**.


## Goal
To build a cloud-native data pipeline that:
- Processes large-scale image feature data in a distributed environment  
- Applies dimensionality reduction using PySpark  
- Demonstrates model weight distribution across compute nodes  
- Ensures compliance with GDPR-aligned data handling practices  
- Optimizes infrastructure for cost-efficient execution  


## Architecture Components

### 1. AWS EMR Cluster
- Scalable distributed compute environment  
- Region-restricted deployment (EU compliance considerations)  

### 2. PySpark Processing Layer
- Distributed feature processing  
- PCA-based dimensionality reduction at scale  

### 3. Model Distribution Layer
- TensorFlow model weight broadcasting across cluster nodes  
- Efficient memory-aware computation strategy  


## Key Implementations

- `pca_reduction.py`  
  Distributed PCA using PySpark for feature compression  

- `broadcast_model.py`  
  TensorFlow weight broadcasting across EMR nodes  

- `emr_setup.md`  
  Step-by-step AWS EMR cluster deployment guide  


## Data Processing Pipeline
1. Data ingestion into AWS S3  
2. EMR cluster initialization  
3. Distributed preprocessing with PySpark  
4. Dimensionality reduction (PCA)  
5. Model distribution and execution across nodes  
6. Output storage for downstream ML tasks  


## Key Concepts Demonstrated
- Cloud-native distributed computing (AWS EMR)  
- Big data processing with PySpark  
- Model parameter distribution in cluster environments  
- Dimensionality reduction at scale  
- GDPR-aware infrastructure design  
- Cost-efficient ML system design  


## Technical Stack
AWS EMR • PySpark • TensorFlow • Python • S3

---

## Key Takeaways
- Practical experience with distributed data processing systems  
- Understanding of scalable ML infrastructure design  
- Trade-offs between compute cost and processing efficiency  
- Importance of data governance in cloud-based systems  


##  Contents

```
FruitsAI-Cloud-Pipeline/
├── pca_reduction.py              # Dimensionality reduction with PySpark
├── broadcast_model.py           # TensorFlow weights distribution logic
├── emr_setup.md                 # Step-by-step guide to launching an EMR cluster
├── sample_notebook.ipynb        # Inherited from former intern, updated and extended
├── data/
│   └── fruits_dataset/          # Sample image and label data
├── docs/
│   └── GDPR_compliance.md       # Hosting & privacy considerations
├── README.md                    # Project overview and goals (this file)
```

##  License

MIT License – use freely with attribution.

