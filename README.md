# Consensus Clustering
A Python + R program for consensus clustering implementation based on  [this paper](https://link.springer.com/article/10.1023/A:1023949509487). 


<p align="center">
  <img src="https://user-images.githubusercontent.com/50635618/170343914-0ec6aa39-b32d-47c3-8aba-c056fd21ec46.png"/>
</p>



## Requirements 
Python packages: matplotlib, pandas, seaborn, numpy, and PIL

R libraries: BiocManager, ConsensusClusterPlus


## Running
I explain the method via an example. Here we have a six clusters data corresponding to 'no artifact', 'other artifacts', 'ringing', 'ghosting', 'banding', and 'motion' classes. The values of the data for each cluster along with the cluster labels is saved in _.txt_ files (see files directory).

### Step 1
The first step is to run the R code named **R**. The input of the script is two _.txt_ files and the output is a _out_text.txt_ file and a folder named "saved_folder" containing the consensus plots. Since here we have six clusters (k=6) we will need the plot named _consensus06.png_ which looks like the follwoing plot. 


<p align="center">
  <img src="https://user-images.githubusercontent.com/50635618/170344444-b230fb3d-ce3c-4034-92d6-442be4425fbb.png"/>
</p>

### Step 2
The second step is to run the Python code named **P**. The input of the script is the _out_text.txt_ file and the output is a _report.xlsx_ file and three _.png_ plots as follows.   


![DL+IQMs_whole_labels](https://user-images.githubusercontent.com/50635618/170344968-5bed9e71-498a-4c3b-aa6e-d7c9c86d52cb.png)

![DL+IQMs_labels](https://user-images.githubusercontent.com/50635618/170344981-3fa8b78b-bf26-4dbf-a21f-a161310c6ed1.png)


![DL+IQMs](https://user-images.githubusercontent.com/50635618/170344990-6152656b-23d5-4d1d-b0e2-cbac85c5dbc6.png)



