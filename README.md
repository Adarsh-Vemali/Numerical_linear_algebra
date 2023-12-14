# Node Representation Learning in Graphs
## Course: DSC 210 FA’23 Numerical Linear Algebra
## Instructor: Dr. Tsui-wei Weng
Code for the Numerical Linear Algebra project on Graphs

This repository consists of 3 ipython notebooks for:-
1) Laplacian Eigenmaps  : Cora_Eigenmap.ipynb
2) Randomwalks          : Cora_Deepwalk.ipynb         
3) SOTA GCNN Approach   : SOTA_GCN_Approach.ipynb  

The file _requirements.txt_ contains the dependencies required to run the code (The code itself takes care of installing and importing these dependencies).
# Instructions to Run the Code on Colab
1. Open notebook in Colab, Click on the .ipynb file and then Open in Colab
2. Change runtime type to T4 GPU, Runtime => Hardware Accelerator => T4 GPU
3. Run all the cells, Runtime => Run all

### Results:

Following is the visualization for the embeddings that were generated for various classes in the Numerical Linear Algebra based and the Graph Convolutional Neural Network based approaches. 

<img width="350" alt="Untitled" src="https://github.com/Adarsh-Vemali/Numerical_linear_algebra/assets/68332419/40f90667-2266-4237-ac70-8d7de442381b">
<img width="350" alt="Untitled" src="https://github.com/Adarsh-Vemali/Numerical_linear_algebra/assets/68332419/af28fa1f-de82-44bb-bb6c-51a9143004f7">

           Fig. 3.5.1. NLA Approach                   Fig. 3.5.2. SOTA Approach

| Model              | Training time           | Inference time (/ sample) | Accuracy (%) | F1-Score |
|--------------------|-------------------------|---------------------------|--------------|----------|
| Laplacian Eigenmap | 60s (59.8 NLA + 0.2 ML) | 7.4 µs                    | 77.3         | 0.77     |
| Deep Walk          | 19s (18 NLA + 1 ML)     | 7.4 µs                    | 70.0         | 0.69     |
| GCN                | 13.48s                  | 40 µs                     | 81.8         | 0.82     |
