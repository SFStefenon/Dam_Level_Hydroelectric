# Dam Level in a Hydroelectric Power Plant During a Flood

The recorded data presented here, are based on information from the **automatic hydraulic control** for the month of July 2020. 
In this period there was a **flood** going **from 20.46%** of the useful volume of the dam **to 86.27%** in less than **20 days**. 
The records were recorded at a time interval of 1h, for 31 days, corresponding to 744 records.

**Barra Grande** hydroelectric power plant is located on the Pelotas River, about 43 kilometers from its confluence with the Canoas River, between the cities of Anita Garibaldi/SC and Pinhal da Serra/RS, Brazil.
https://www.baesa.com.br/

This power plant has an installed capacity of **690MW**, with a **94km² reservoir** and a **185m high dam**. Based on its characteristics, it has a capacity equivalent to 24% of the demand in the state in which it is installed (Santa Catarina state, Brazil).

To perform an evaluation of the possible scenarios in a sequence-to-sequence (Seq2Seq) time series, noise is included randomly. Using this data, it is possible to evaluate the original signal, as well as two possible scenarios with higher noise intensity (_x1_ and _x2_), as can be seen:

![image](https://user-images.githubusercontent.com/88292916/223682353-37184d39-a204-498d-8153-c7dcba5305c6.png)

# Wavelet-Seq2Seq-LSTM with Attention model

This repository presents an algorithm called Wavelet-Seq2Seq-LSTM with Attention.

> The wavelet transform makes noise reduction for chaotic time series.

> The seq2seq-LSTM makes predictions based on the history of variation in the dam level of the hydroelectric plant.

> The attention mechanism assigns appropriate weight to each encoder's hidden state output, and maps them to the output sequence, solving the problem of having a weak memory about the previous time steps in a long time series.

The notebook for the analysis is divided according to the evaluations:

> Seq2Seq-LSTM with Attention: Evaluation of the starting model using the Attention Mechanism.

> Optimized Seq2Seq-LSTM with Attention: Evaluation with the optimized hyperparameters (based on Optuna).

> Standard Seq2Seq LSTM: Standard model for comparative purposes.

Please go ahead and try it on [Google Colab](https://colab.research.google.com/github/SFStefenon/EWT-Seq2Seq-LSTM-Attention/blob/main/EWT_Seq2Seq_LSTM_Attention.ipynb)!

![image](https://user-images.githubusercontent.com/88292916/223674069-708ecf87-0bac-4abe-a16c-df7b05013a0f.png)

---

Wrote by Dr. Stefano Frizzo Stefenon and Dr. Laio Oriel Seman.

Trento, Italy, March 10, 2023.
