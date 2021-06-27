# GRU-LSTM-FED
Python implementation NASDAQ-100 price prediction using FED's assets 
Based on the work "Predicting Stock Price using LSTM model, PyTorch" by Taron Zakaryan, Paris, Île-de-France, France
Project site can be found here: https://www.kaggle.com/taronzakaryan/predicting-stock-price-using-lstm-model-pytorch

The Federal Reserve System (also known as the Federal Reserve or simply the Fed) is the central banking system of the United States of America.

Since the corona-virus pandemic broke, the United States Federal Reserve 
assets nearly doubled, which raised claims that the Fed is inflating the value of assets in the stock market.

In our project we will examine this claim. We will do so by implementing 2 different methods for RNN models, and compare their results with
each other and examine the influence of the FED's assets on the results.

We can divide the workflow into few main steps:

Loading the data.
Spliting the data.
Building the LSTM and GRU models.
Using OPTUNA for tuning of hyper parameters.
Compering the results with themselves and with the naive prediction (average weekly gain).
Presenting the results.

Parameters
kernel_size = size of the line segement kernel (usually 1/30 of the height/width of the original image)
stroke_width = thickness of the strokes in the Stroke Map (0, 1, 2)
num_of_directions = stroke directions in the Stroke Map (used for the kernels)
smooth_kernel = how the image is smoothed (Gaussian Kernel - "gauss", Median Filter - "median")
gradient_method = how the gradients for the Stroke Map are calculated (0 - forward gradient, 1 - Sobel)
rgb = True if the original image has 3 channels, False if grayscale
w_group = 3 possible weight groups (0, 1, 2) for the histogram distribution, according to the paper (brighter to darker)
pencil_texture_path = path to the Pencil Texture Map to use (4 options in "./pencils", you can add your own)
stroke_darkness = 1 is the same, up is darker.
tone_darkness = as above
Folders
inputs: test images from the publishers' website: http://www.cse.cuhk.edu.hk/leojia/projects/pencilsketch/pencil_drawing.htm
pencils: pencil textures for generating the Pencil Texture Map
Reference
[1] Lu C, Xu L, Jia J. Combining sketch and tone for pencil drawing production[C]//Proceedings of the Symposium on Non-Photorealistic Animation and Rendering. Eurographics Association, 2012: 65-73.

[2] Matlab implementation by "candtcat1992" - https://github.com/candycat1992/PencilDrawing
