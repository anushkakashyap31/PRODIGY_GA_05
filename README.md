> # **🚀 PRODIGY_GA_05 — Neural Style Transfer using TensorFlow Hub**

This repository contains **Task 5: Neural Style Transfer** Project as part of my **Generative AI Internship** at **Prodigy Infotech**, where I applied the artistic style of a painting to the content of another image using a pre-trained model from TensorFlow Hub.

### **💡 Project Overview**

In this task, I have:

- Used **TensorFlow** and TensorFlow Hub to perform Neural Style Transfer.
- Combined the content of one image with the style of another to generate a stylized image.
- Worked on **Google Colab** for easy access and GPU acceleration.

### **📄 Files**

- `Task_5_Neural_Style_Transfer.ipynb`: The complete Colab notebook.
- `stylized_output.jpg`: Example stylized image output.
- `sample_images/`: Folder containing the content and style images.
- `.gitignore`: Skips unnecessary files in version control.
- `README.md` File

### **⚙️ Technologies Used**

- Python
- Google Colab
- Tensorflow
- Matplotlib
- Numpy

### **💬 How to Use**

1️⃣ Open the notebook in Google Colab: [🔗][https://colab.research.google.com/drive/1-wsnpwTzuOrLi9jBJHQKhq3dd2mYpL5r]

✅ STEP 1: Install Required Libraries

```
!pip install tensorflow matplotlib tensorflow_hub
```

✅ STEP 2: Load and Preprocess Images

```
def load_img(path_to_img):
    # Load, decode, normalize, resize, and batch the image
    ...
```

✅ STEP 3: Load Pre-trained Model and Stylize

```
import tensorflow_hub as hub

# Load model
hub_model = hub.load('https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2')

# Apply style
stylized_image = hub_model(tf.constant(content_image), tf.constant(style_image))[0]
```

✅ STEP 4: Display and Save Output

```
# Display stylized image
imshow(stylized_image, 'Stylized Image')

# Save output
image = tensor_to_image(stylized_image)
image.save("stylized_output.jpg")
```


2️⃣ Upload your own content and style images if desired.
3️⃣ Run all cells to see the final result.



### **🎯 Objectives**

- Learn to blend artistic style with content using deep learning.
- Understand and utilize TensorFlow Hub’s pre-trained models.
- Apply computer vision techniques practically using Colab.

### **👩‍💻 Author**

### **Anushka Kashyap**

### **⭐ Acknowledgements**

- Prodigy Infotech
- Tensorflow Hub
- Google Colab
- Magenta Team (for the pre-trained model)


**✨ Do ⭐ star the repo if you found it useful!**
