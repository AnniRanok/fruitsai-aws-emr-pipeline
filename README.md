
# Cloud Data Processing & Distributed ML Pipeline (AWS EMR + PySpark)

## Project Overview
This project focuses on designing a scalable cloud-based data processing and distributed ML pipeline using AWS EMR and PySpark.

The system demonstrates how large-scale datasets can be processed in a distributed environment with emphasis on **scalability, cost efficiency, and privacy-aware data handling**.

The architecture is designed for **cloud-native batch processing and feature engineering workflows**.


## Goal
To build a cloud-based distributed data processing pipeline that:

- Processes large-scale datasets in a distributed environment  
- Applies dimensionality reduction using PySpark (PCA)  
- Demonstrates model weight distribution across compute nodes  
- Implements GDPR-aligned data handling practices  
- Optimizes infrastructure for cost-efficient execution  


## Architecture Components

### 1. AWS EMR Cluster
- Scalable distributed compute environment  
- Region-restricted deployment (EU compliance-ready setup)  
- Designed for batch processing workloads  

### 2. PySpark Processing Layer
- Distributed feature processing  
- PCA-based dimensionality reduction at scale  

### 3. Model Distribution Layer
- TensorFlow model weight broadcasting across EMR nodes  
- Memory-efficient distributed execution strategy  


## Key Implementations

- `pca_reduction.py`  
  Distributed PCA implementation using PySpark for feature compression  

- `broadcast_model.py`  
  TensorFlow model weight distribution across cluster nodes  

- `emr_setup.md`  
  AWS EMR cluster deployment and configuration guide  


## Data Processing Pipeline
1. Data ingestion into AWS S3  
2. EMR cluster initialization  
3. Distributed preprocessing with PySpark  
4. Dimensionality reduction (PCA)  
5. Model distribution across nodes  
6. Output storage for downstream ML workflows  

---

## Key Concepts Demonstrated
- Cloud-native distributed computing (AWS EMR)  
- Big data processing with PySpark  
- Distributed model execution strategies  
- Dimensionality reduction at scale  
- Data governance and GDPR-aligned design principles  
- Cost-efficient cloud architecture design  


## Technical Stack
AWS EMR • PySpark • TensorFlow • Python • AWS S3  


## Key Takeaways
- Practical experience with distributed data processing systems  
- Design of scalable cloud-based ML pipelines  
- Trade-offs between compute cost and system performance  
- Data governance considerations in cloud environments  
- End-to-end understanding of batch processing architectures  


## Project Structure

```
FruitsAI-Cloud-Pipeline/
├── pca_reduction.py             # Dimensionality reduction with PySpark
├── broadcast_model.py           # TensorFlow weights distribution logic
├── emr_setup.md                 # Step-by-step guide to launching an EMR cluster
├── sample_notebook.ipynb        # Inherited from former intern, updated and extended
├── data/
│   └── fruits_dataset/          # Sample image and label data
├── docs/
│   └── GDPR_compliance.md       # Hosting & privacy considerations
├── README.md                    # Project overview and goals (this file)
```

## License
MIT License

