# COMP7103C-Project
LSTM.ipynb is the code for LSTM model.

CNNStock.ipynb is the code for CNN model.

These codes can be run in order.


# CNN

Pytorch code for the CNN model of stock tendency prediction in jupyter notebook.

Testing Enviroment:
Python 3.6
PyTorch 1.6.0
CUDA 10.1

CNNStock.ipynb contains data processing, model construction, model training, strategy construction, strategy backtest, result graph drawing. Every section has corresponding code comments.
The input data is saved locally by
np.save('train_x_20D_HSI',train_x)
np.save('train_y_20D_HSI',train_y)
np.save('test_x_20D_HSI',test_x)
np.save('test_y_20D_HSI',test_y) 
Model parameters is saved by
torch.save(para_dict, "./Net_20D_V2_HSI_1.pkl")
True price and prediction result for backtest is saved by 
	true_price.to_csv('true_price_20D_V2_HSI_1.csv')
pred_prob.to_csv('pred_prob_20D_V2_HSI_1.csv')
