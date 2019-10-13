# Cats_and_dogs

Data: https://www.kaggle.com/c/dogs-vs-cats/data \
Loaded to google drive to folder /content/drive/My Drive/datasets/dogscats/ \
The training data contains 12500 images of each class. \
12000 images in training set, 500 images in validation set. 

Trials: \
1: Original data, Resize to 448x448, reached 85% accuracy \
2: Blur effect of size 10x10. Resize to 450x450, reached above 75% \
  Model:  \
    Kernel of 4x4 out 10 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 20 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 40 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 80 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 160 channels, padding=1, maxpool of size (2x2) \
    FC layer, out 500  \
    FC layer, out 10 \
2 with 6 layers: Blur effect of size 10x10. Resize to 450x450, reached 50% \
  Model:  \
    Kernel of 4x4 out 10 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 20 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 40 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 80 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 160 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 320 channels, padding=1, maxpool of size (2x2) \
    FC layer, out 500  \
    FC layer, out 10 \
2 more channels:Blur effect of size 10x10. Resize to 450x450, reached 70% \
  Model:  \
    Kernel of 4x4 out 20 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 40 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 80 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 160 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 320 channels, padding=1, maxpool of size (2x2) \
    FC layer, out 500  \
    FC layer, out 10 \
3: Blur effect of size 10x10. Resize to 450x450, removed 1000 images from each class \
  Model:  \
    Kernel of 4x4 out 10 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 20 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 40 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 80 channels, padding=1, maxpool of size (2x2) \
    Kernel of 4x4 out 160 channels, padding=1, maxpool of size (2x2) \
    FC layer, out 500  \
    FC layer, out 10 \
4: Blur effect of size 10x10. Resize to 450x450, removed 2000 images from each class \
  Model: \
    Kernel of 3x3 out 32 channels, padding=1 \
    Kernel of 3x3 out 32 channels, padding=1 \
    maxpool of size (2x2) \
    Kernel of 3x3 out 64 channels, padding=1 \
    Kernel of 3x3 out 64 channels, padding=1 \
    maxpool of size (2x2) \
    Kernel of 3x3 out 128 channels, padding=1 \
    Kernel of 3x3 out 128 channels, padding=1 \
    maxpool of size (2x2) \
    Kernel of 3x3 out 256 channels, padding=1 \
    Kernel of 3x3 out 256 channels, padding=1 \
    maxpool of size (2x2) \
    FC layer, out 256, dropout of 0.5 \
    FC layer, out 256, dropout of 0.5 \
    FC layer, out 10     \
5: Blur effect of size 10x10. Resize to 450x450, removed 3000 images from each class \
  Model: \
    Kernel of 3x3 out 32 channels, padding=1 \
    Kernel of 3x3 out 32 channels, padding=1 \
    maxpool of size (2x2) \
    Kernel of 3x3 out 64 channels, padding=1 \
    Kernel of 3x3 out 64 channels, padding=1 \
    maxpool of size (2x2) \
    Kernel of 3x3 out 128 channels, padding=1 \
    Kernel of 3x3 out 128 channels, padding=1 \
    maxpool of size (2x2) \
    Kernel of 3x3 out 256 channels, padding=1 \
    Kernel of 3x3 out 256 channels, padding=1 \
    maxpool of size (2x2) \
    FC layer, out 256, dropout of 0.5 \
    FC layer, out 256, dropout of 0.5 \
    FC layer, out 10 \
6: Blur effect of size 10x10. Resize to 450x450, removed 4000 images from each class NOT FINISHED RUNNING \
  Model: \
    Kernel of 3x3 out 32 channels, padding=1 \
    Kernel of 3x3 out 32 channels, padding=1 \
    maxpool of size (2x2) \
    Kernel of 3x3 out 64 channels, padding=1 \
    Kernel of 3x3 out 64 channels, padding=1 \
    maxpool of size (2x2) \
    Kernel of 3x3 out 128 channels, padding=1 \
    Kernel of 3x3 out 128 channels, padding=1 \
    maxpool of size (2x2) \
    Kernel of 3x3 out 256 channels, padding=1 \
    Kernel of 3x3 out 256 channels, padding=1 \
    maxpool of size (2x2) \
    FC layer, out 256, dropout of 0.5 \
    FC layer, out 256, dropout of 0.5 \
    FC layer, out 10 \
7: Blur effect of size 10x10. Resize to 450x450, removed 2000 images from each class \
  Model: \
    Kernel of 16x16 out 20 channels, padding=1, maxpool of size (2x2) \
    Kernel of 16x16 out 40 channels, padding=1, maxpool of size (2x2) \
    Kernel of 16x16 out 60 channels, padding=1, maxpool of size (2x2) \
    Kernel of 16x16 out 80 channels, padding=1, maxpool of size (2x2) \
    FC layer, out 500  \
    FC layer, out 10 \
