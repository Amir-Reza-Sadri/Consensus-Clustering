# Consensus Clustering
A Python + R program for consensus clustering implementation based on  [this paper](https://link.springer.com/article/10.1023/A:1023949509487). 


<p align="center">
  <img src="https://user-images.githubusercontent.com/50635618/170381479-1485dd6a-7a9a-49bc-a514-bdbb42c15729.png"/>
</p>



## Requirements 
Python packages: matplotlib, pandas, seaborn, numpy, and PIL

R libraries: no specific library is needed


## Running
I explain the method via an example. Here we have a six clusters data corresponding to 'no artifact', 'other artifacts', 'ringing', 'ghosting', 'banding', and 'motion' classes. The values of the data for each cluster along with the cluster labels is saved in _.txt_ files (see files directory).

### Step 1
The first step is to run the R code named **R**. The input of the script is two _.txt_ files and the output is a _out_text.txt_ file and a folder named "saved_folder" containing the consensus plots. Since here we have six clusters (k=6) we will need the plot named _consensus06.png_ which looks like the follwoing plot. 


<p align="center">
  <img src="https://user-images.githubusercontent.com/50635618/170381567-b285503e-dce4-4cef-a0bf-10c7cca6ac56.png"/>
</p>

### Step 2
The second step is to run the Python code named **P**. The input of the script is the _out_text.txt_ file and the output is a _report.xlsx_ file and three _.png_ plots as follows.   

![Picture2](https://user-images.githubusercontent.com/50635618/170382491-ef2400ea-cdfe-492f-982a-b8170496c3b9.png)


The metrics of each cluster is in the following format.

| ClassNumber    | ClassName     | TP         | FP | TN | FN | Accuracy | Recall  | Precision | 
| ------------- | ------------- | --------    |------------- | ------------- | --------    |------------- | ------------- | --------    |
| 5     | banding        | 9  | 0 | 90 | 1 | 0.99 | 0.9 | 1| 
| 1     | bno artifact        | 31  | 2 | 66 | 1 | 0.97 | 0.97 | 0.94| 
| 2     | other artifacts       | 2  | 0 | 97 | 0 | 1 | 1 | 1| 
| 3     | ringing      | 16 | 1 | 82 | 4 | 0.95 | 0.8 | 0.94| 
| 6     | motion       | 12  | 1 | 86 | 3 | 0.96 | 0.8 | 0.92| 
| 4     | ghosting        | 20  | 5 | 74 | 0 | 0.95 | 1 | 0.8| 

### Step 3
Finally, a _.pptx_ file is made to visualize the whole result. 
