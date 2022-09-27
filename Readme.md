# Bark Texture Images Classification

This is Solution for the Task given for fellowship

The Model has

1.Training Accuracy : 96.76

2.Testing Accuracy : 91.32

The Model is Trained the [Dataset](https://www.kaggle.com/datasets/saurabhshahane/barkvn50) by Transfer Learning with  the [VGG16](https://arxiv.org/abs/1409.1556v6) with keras

## Idea Behind This

Data is images with size 303× 404 of 5,578 images.The First is to split the dataset into test,train and validation split.
After Splitting the Data .Next is to Resize the image to 224x224 using keras's load_image function is it is being trained on VGG16,which originally trained 224x224 imagenet dataset. Later with Transer Learning  ,making the layers of VGG16 non trainable and added few dense layers for classfication with softmax as output activation layer.with this we are able to achieve 96.76 training accuracy.For avoiding the Overfitting used Dropout layer.

## Model Architecture

[![image.png](https://i.postimg.cc/PxXSmrWz/image.png)](https://postimg.cc/LqWkSS0n)

## Results 

[![image.png](https://i.postimg.cc/5t60j8Gw/image.png)](https://postimg.cc/Z9zZMvJR)

[![image.png](https://i.postimg.cc/65tpnkg6/image.png)](https://postimg.cc/G9gR15b6)

## Run Locally

To deploy this project run

```python
    pip install -r requirements.txt
```

Run Jupyter Notebook

## Demo

This is Deployed on Huggingface spaces.

[View Here](https://huggingface.co/spaces/eswardivi/Bark_Texture_Images_Classification)

[![image.png](https://i.postimg.cc/3xs0H4yn/image.png)](https://postimg.cc/CR4xGKsq)
