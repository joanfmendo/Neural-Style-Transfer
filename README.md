# Neural-Style-Transfer
Following Vamshik Shetty's tutorial, this post applies the use of convolutional neural networks to "transfer style" from one image to another. What would a picture of your pet look like if it had been painted by Picasso? Let's find out!

This is a simple script on how to use some convolutional neural networks to "transfer the style" of one picture to another. It is very simple to implement and very easy to understand.

**I strongly recommend using Google Colab** to run these scripts, since neural networks require a lot of computing and memory capacity. The best thing is that GColab is free!! You can find a tutorial [here](https://medium.com/deep-learning-turkey/google-colab-free-gpu-tutorial-e113627b9f5d).

**HOW TO USE THIS SCRIPT**

First, pick up two images, one is the photo that you want to modify (it is, the one you will apply the new style), and the other contains the style that you want to apply (or to "transfer").

Next, go to these lines and modify them indicating the path to your images.

`# Set up paths to style and content files`

`style_path = '/path-to-the-file/style.jpg'` Image containing the "style".

`content_path = '/path-to-the-file/content.jpg'` Image containing the content you want to modify by applying the selected style.

Then, modify the size of the output file (in pixels) and the number of epochs (iterations) of the CNN algorithm.
`# Set up the maximum dimension of the output image`

`max_dim = 1500` Maximum size of the output file in pixels

`# set up the number of iterations`

`num_iter = 500` Number of epochs of the training algorithm.

In my case, I used a photo I took of a beautiful friend (her name is Monica. Btw I'm a photographer in case you don't know) and I applied Van Gogh's "Starry Night" style.

![alt text](https://github.com/joanfmendo/Neural-Style-Transfer/blob/master/example.png)

After 500 epochs, the final result looks like this:
![alt text](https://github.com/joanfmendo/Neural-Style-Transfer/blob/master/output.png)
