# Time Series for MQL5

This is a Time Series Library tailor-made for MQL5. This Library is designed to handle some useful operations regarding Time Series dataset. 

The array of features includes:
   ```void     PlotDataset(matrix &dataset,int colum);```

   ```void     PlotTest(matrix &y_true, matrix &y_pred);```

   ```matrix   ReadDataset(string M_name);```

   ```void     WriteDataset(matrix &M, string M_name);```

   ```matrix   Features(ulong i,ulong N_steps, matrix &M);```

   ```matrix   RealOutput(ulong i, ulong j, ulong N_steps, matrix &M);```

   ```matrix   OutputTest(int j, ulong N_steps, matrix &M_test);```

   ```matrix   NormalizeDataset(matrix &dataset);```

   ```matrix   DatasetTest(matrix &dataset, double percentage);``` 

   ```matrix   DatasetTrain(matrix &dataset, double percentage);```

