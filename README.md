<img src="https://github.com/joaopaulo-souza/Time-Series-for-MQL5/blob/master/robot-timeseries.jpeg">

# Time Series for MQL5

This is a Time Series Library tailor-made for MQL5. This Library is designed to handle some useful operations regarding Time Series dataset. 

The file TimeSeriesData.mqh is supposed to be in the include directory of MetaTrader5

The array of features includes:

   ```void     PlotDataset(matrix &dataset,int colum);```
This is used to plot a graph of a specific feature of the dataset
The int column parameter is the specific feature

   ```void     PlotTest(matrix &y_true, matrix &y_pred);```
This is used to plot a graph with the predicted values and the true values
y_pred is the predicted values, and y_true is the true values

   ```matrix   ReadDataset(string M_name);```
This is used to read some dataset given in .csv file and return the corresponding matrix
M_name is the name of the .csv file

   ```void     WriteDataset(matrix &M, string M_name);```
This is used to write some matrix in a .csv file 
M is the matrix, M_name is the name of the .csv file

   ```matrix   Features(ulong i,ulong N_steps, matrix &M);```
This is used to get some sample in a time series dataset 
Where i is the index of the sample, N_steps is the number of time steps the sample has

   ```matrix   RealOutput(ulong i, ulong j, ulong N_steps, matrix &M);```
This is used to return the real value of the dataset given a sample
Where i is the index of the sample, j is the feature's index to be predicted, 
N_steps is the number of time steps of each sample and M is the dataset

   ```matrix   OutputTest(int j, ulong N_steps, matrix &M_test);```
Returns the matrix with the real outputs given a test dataset

   ```matrix   NormalizeDataset(matrix &dataset);```
This is used to normalize the dataset. 

   ```matrix   DatasetTest(matrix &dataset, double percentage);```
This is used to split the dataset. It returns the train dataset 
The percentage is the percentage of the dataset used for training

   ```matrix   DatasetTrain(matrix &dataset, double percentage);```
This is used to split the dataset. It returns the test dataset 
The percentage is the percentage of the dataset used for test
