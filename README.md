# Image-Classification-Using-Deep-Learning
Multi-label Image Classification using Automated Approach.

# Dataset
The complete description of dataset is given on http://lamda.nju.edu.cn/data_MIMLimage.ashx. The dataset contains 2000 natural scenes images.

# Preprocessing
Resized all images to 100 by 100 pixels and created two sets i.e train set and test set. Train set contains 1600 images and test set contains 200 images.

# Training
As this is multi label image classification, the loss function was binary crossentropy and activation function used was sigmoid at the output layer. Keras doesn't have provision to provide multi label output so after training there is one probabilistic threshold method which find out the best threshold value for each label seperately, the performance of threshold values are evaluated using Matthews Correlation Coefficient and then uses this thresholds to convert those probabilites into one's and zero's.

# Visualization
Command:
python visualization.py
link: localhost:5000

# Keras repo
Github: https://github.com/keras-team/keras

# License
This code is provided under the MIT License.

Copyright 2019 Yasrub Bashir Malik

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
