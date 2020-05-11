# Leveraging Transfer Learning to Imitate Human Behaviour for Image Colorization

We implemented an Ensemble model for image colorization, the task of generating colored images from grayscale image inputs.

- We built upon the work by Melas-Kyriazi and Han [1]
- We leveraged transfer learning for the classification, Alexnet [2]

By treating image colorization as a classification task and using other advancements, the best results are possible [4]. Regression task settings are easier but perform worse [3]. We tried to imitate human behavior, first classify the scene and then choose sensible colors, with a regression-based (MSE loss) Ensemble model that adds separated classification results as mid-features (Fusion Layer).

For the source information see the [poster](./poster-image-colorization.pdf).