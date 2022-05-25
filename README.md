# Consensus Clustering
A Python + R program for consensus clustering implementation based on  [this paper](https://link.springer.com/article/10.1023/A:1023949509487). 


<p align="center">
  <img src="https://user-images.githubusercontent.com/50635618/170316194-cf1be8b8-8772-4e28-b270-e2d75386ba8b.png"/>
</p>



## Requirements 
Python packages: matplotlib, pandas, seaborn, numpy, and PIL

R libraries: BiocManager, ConsensusClusterPlus


## Running
I explain the method via an example. Here we have a six clusters data corresponding to 'no artifact', 'other artifacts', 'ringing', 'ghosting', 'banding', and 'motion' classes. The values of the data for each cluster along with the cluster labels is saved in _.txt_ files (see files directory).

### Step 1
The first step is to run the R code named R. The input of the script is two _.txt_ files and the output is a _out_text.txt_ file and a folder named "saved_folder" containing the consensus plots. Since here we have six clusters (k=6) we will need the plot named _consensus06.png_ which looks like the follwoing plot. 


<p align="center">
  <img src="https://user-images.githubusercontent.com/50635618/170335825-e24077b5-5c93-41e2-b7e2-24699c0455ba.png"/>
</p>

