# Cats_and_dogs

Data: https://www.kaggle.com/c/dogs-vs-cats/data
Loaded to google drive to folder /content/drive/My Drive/datasets/dogscats/

Trials:
1. Original data, Resize to 448x448, reached 85% accuracy
2. Blur effect of size 10x10. Resize to 450x450, reached above 75%
Model: Kernel of 10x4x4, padding=1. 
  Kernel of 4x4 out 20 channels, padding=1
  Kernel of 4x4 out 40 channels, padding=1
  Kernel of 4x4 out 80 channels, padding=1
  Kernel of 4x4 out 160 channels, padding=1
  FC layer, out 500 
  FC layer, out 10
3. 
