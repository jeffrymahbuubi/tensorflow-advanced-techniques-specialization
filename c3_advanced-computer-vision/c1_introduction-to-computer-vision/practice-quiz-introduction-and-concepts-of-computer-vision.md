## Practice Quiz: Introduction and Concepts of Computer Vision

### Question 1

In a Multi-Class classification scenario, your model can identify all the different items and people that are present in a given input image

- True
- **False**

> Correct! The above statement is true for a Multi-Label Classification

### Question 2

Which of the following statements correctly describes the difference between object detection and object localization?

- _Object detection_ refers to detecting the object within an image, while object localization gives us the bounding box around that object.
- They both are the same.
- **_Object localization_ is where you get a bounding box around the main subject of the image, while in object detection you get a bounding box around all of the objects within an image.**
- _Object detection_ is where you get a bounding box around the main subject of the image, while in object localization you get a bounding box around all of the objects within an image.

> Correct

### Question 3

What is the method that locates an object(s) by labelling the pixels, where each similar object(s) is assigned to the same class? Type your response here (two words, all lower case) **Semantic Segmentation**

> Correct

### Question 4

In the context of _Transfer Learning_, the initial training task where the model learns reusable patterns is called a _downstream task_

- True
- **False**

> Correct! The above statement is true for a _pre-trainint task_. The task for which the model is borrowed is called _downstream task_

### Question 5

Check all the scenarios in which Transfer Learning could be beneficial.

- **When the task you want to perform is a sub-task of an already trained, larger, model.**

> Correct

- To ensure better performance
- **To reduce computation and processing cost**

> Correct

- **When you don't have enough data for the task you want to perform, which resembles another same or similar, already trained task.**

> Correct

### Question 6

What is the name of built-in TensorFlow layer-type which you can use to increase the dimensions of a 2D image?

- SampleUp2D
- UpSampling
- SampleIncrease
- **UpSampling2D**

> Correct

### Question 7

You have an image of dimensions 48 x 48, and you want to upscale it to 240 x 240 using built-in TensorFlow layer-type which is used to perform such as task (mentioned in Question 6). What will you pass in as size? **(5, 5)**

> Correct

### Question 8

Consider the following code:

```python
my_layer = tf.keras.applications.resnet.ResNet50(
    input_shape=(224,224,3),
    include_top=False,
    weights='imagenet'
)(inputs)
```

What does "include_top=False" mean?

- It discards the first layer of ResNet50 when initializing my_layer using it.
- It sets the top most layers as untrainable of ResNet50 when initializing my_layer using it.
- **It discards the top most layers of ResNet50 when initializing my_layer using ResNet50.**
- It randomly sets up the weights, instead of using that of ImageNet, for the top most dense layers of ResNet50 when initializing my_layer using it.

> Correct

### Question 9

What is the name of the technique used in the output dense layer that is used to predict Bounding Boxes? Hint: It is a one word answer **Regression**

> Correct

### Question 10

Check all the statements that are true regarding Intersection Over Union (IoU), with regards to Bounding Boxes.

- **IoU is the area of intersection of the two boxes (true and predicted) divided by the total union area of the two boxes.**

> Correct

- The closer the value of loU is to 0 the better is the prediction of the bounding box.
- **The closer the value of loU is to 0 the poorer is the prediction of the bounding box.**

> Correct The lesser the area of intersection the closer to 0 will be the value of IoU

- The values of loU range from 0 to all possible positive values.
