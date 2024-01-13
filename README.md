# Handwritten Gplyph Classification | TMNIST

Handwritten character Classification is a fundamental example in the field of Computer Vision. It is the process of developing the capabilities for machines to understand handwritten characters and digits, which has various applications ranging from Biometrics to creation of Digital Libraries. In this notebook we build specific type of neural network called [Convolutional Neural Network](https://en.wikipedia.org/wiki/Convolutional_neural_network) (CNN)  - commonly used for image classification projects - to classification digits and characters. For this tutorial, we will an use extended version of the classification MNIST dataset - [TMIST](https://www.kaggle.com/datasets/nimishmagre/tmnist-glyphs-1812-characters/data).

# Dataset
## TMNIST (Typography MNIST) Glyphs:

This dataset is taken from Kaggle. It has over 500,000 MNIST style images made from 1,819 unique glyphs and 2,990 font-styles

The structure of the csv file is:

* The first row contains column headers ['font_name','glyph_name', 'label','1','2',…..'784']
* The 'font_name' column contains font file names such as 'Acme-Regular' and 'ZillaSlab-Bold'
* The 'glyph_name' column contains the unicodedata name for the glyph such as 'LATIN CAPITAL LETTER A' and 'DEVANAGARI LETTER AA'
* For glyphs that are represented by more than 1 unicode character, the 'glyph_name' column contains the the individual names of both the characters concatenated with a '+' sign. For ex: 'अं' has the 'glyph_name' = 'DEVANAGARI LETTER A + DEVANAGARI SIGN ANUSVARA'
* The 'label' column contains characters such as 'ش','E' or 'छ'
* The remaining 784 columns contain the grayscale pixel values for the image of the corresponding character in the 'font_name' font-style

### Install the necessary libraries

`! pip install tensorflow`


