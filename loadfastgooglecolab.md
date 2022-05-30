# **Load Fast in Google Colab, But Careful...**

We've all been there, Jupyter cannot install a certain package and your project deadline is three hours away. What do you do?

Well, Google colab (short for *Colaboratory*) is the Jupyter but the online version. We just have one major issue... *how to load data*?

In Jupyter, we can simply put the file in the same folder as our notebook and normally load. If the file is in a subfolder, simply change the path in your reader code. But what happens if your notebook is in Google?

We have three approaches when it comes to this, and I'll present the **first** option being the best but **be careful**:

## **Use `gdown`**
With gdown, you can use your dataset in Google drive and the code uploads file from Google drive to colab without the annoying pop-up. Follow the below instructions and be guided accordingly.

### a. Put your dataset in Google drive and make the sharing Public (`Anyone with the Link`)
This is the drawback that if someone gets access to that link, they can download the dataset. Really not wise if you are dealing with private data. Although public folders in google drive is not searcheable, your notebook can if it is public. So if you decide go this route while using sensitive data, make sure your notebook is Restricted.

### b. Get the 'Key'
![image](https://user-images.githubusercontent.com/40331047/170913829-4a0bc3ca-16ee-469a-bf73-d25022d10d93.png)

### c. Insert this code in your Notebook and Run
Observe that upload time is super fast!

![image](https://user-images.githubusercontent.com/40331047/170913660-16019909-7be1-43dc-b25b-613875eb21fb.png)

Voila! You got this.

## Other Methods

### 1 Upload the file and run normally
This would be good but if you close your notebook or reach the 12-hr limit of Google colab/day, then you will need to reupload. Also, upload time takes a lot of time for large files.

![image](https://user-images.githubusercontent.com/40331047/170914309-9c1cf206-02a3-4ac7-876d-81a7cb65a1ee.png)
<br>*In this image, just activate the left pane and drag the files anywhere. Then call the file in the notebook.*

### 2 Put in a Google drive folder
This is the safe way. Although it is pesky that the Google prompt will always pop when you rerun your notebook. But hey, it's safe!

![image](https://user-images.githubusercontent.com/40331047/170916670-e6e63a73-27c8-480e-b3c5-ca24e7d8c0af.png)

<br> These will always appear when you rerun the code... brace yourselves:
![image](https://user-images.githubusercontent.com/40331047/170914768-ee8892f0-ff7c-4d6a-80ed-9deaa7e4b39a.png)
![image](https://user-images.githubusercontent.com/40331047/170914862-490c8f2f-81d8-4d57-8469-4f7f928ad0ae.png)


