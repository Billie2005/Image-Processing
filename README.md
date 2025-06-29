# Image-Processing - 1 
## 1. Basic image handling

(a) Take a high quality, high contrast selfie of yours.

(b) Read and display the image.

(c) If it is a color image, convert it to a grayscale image with an 8 bit representation and store it
as “selfie.jpg”or any other preferred format. Display the image with the colorbar.

(d) What are the number of pixels in each dimension of “selfie.jpg”? Find the minimum and
maximum values of its pixels.

(e) Plot the histogram.

(f) Reduce the bit-representation to 4 bits. In other words, re-quantize the image “selfie.jpg”to 16
grayscale levels. Display the original image and the re-quantized image and comment on the
eﬀect of quantization.


## 2. Intensity transformation

(a) Compute the negative of ‘selfie.jpg’ and display it.

(b) Perform a log transformation of ‘selfie.jpg’. Save it as ‘log selfie.jpg’. Display it and compare
its histogram with that of the original.

(c) Consider the functions T1, T2 and T3 shown in Fig. 1 and perform contrast stretching. Comment
on the diﬀerence between the input and the output image w.r.t the transformations T1, T2 and
T3.
Display the transformed images and compare their histogram with that of the original.

![image](https://github.com/user-attachments/assets/c6285f45-499b-455b-b2f3-2dd86a62243e)

(d) Apply the power law transformation. What happens with diﬀerent values of γ? Compare in
terms of the transformed images and the histograms of the transformed and original images.


(e) Bit-plane Slicing: The 8-bit selfie image may be considered as being composed of eight one-bit
planes, with plane 1 containing the lowest-order bit of all pixels in the image, and plane 8
all the highest-order bits. Display each of these bit-planes separately and comment on the
information present in these bit-planes. Try with diﬀerent images and comment on relative
importance of each bit in the considered image.

## 3. Spatial filtering

(a) Apply the averaging mask (given below) to “selfie.jpg”. Display the output and observe the diﬀerences between the original and the transformed image. What happens as you increase the size of the mask (5 5, 25 25, 51 51 etc)?

![image](https://github.com/user-attachments/assets/fd361d85-4f63-46cc-9c7e-2f29d18c91aa)

(b) Take an asymmetrical mask/filter and demonstrate/verify that correlation is not commutative
while convolution is commutative.

(c) Apply Gaussian filters (of diﬀerent size and variance) to “selfie.jpg”and comment on the eﬀect
of smoothing w.r.t kernel size and variance.

(d) Apply min, max and median filters to “selfie.jpg”and comment on the diﬀerence between the
output images. If the diﬀerence is not clearly visible, choose an image such that the diﬀerence
in output images are clearly distinguishable.

(e) Apply the Laplacian mask (given below) to “selfie.jpg”. Display the output and comment on
the edge enhancing properties of the mask.

![image](https://github.com/user-attachments/assets/bf91df88-e6a4-4ec8-ba5f-f7dbb99a8e95)

(f) Sharpen “selfie.jpg”using unsharp masking. Display the output and observe the diﬀerences
between the original and the transformed image.

(g) Apply Roberts cross-gradient and Sobel operators on “selfie.jpg”and comment on the trans-
formed images.

(h) What are the eﬀects of applying the following masks to “selfie.jpg”? What are the diﬀerences
in the 4 transformed images?

![image](https://github.com/user-attachments/assets/3f8f7e25-b08d-4a24-851e-febd851e1efe)

Choose a suitable image from the internet/web which clearly shows the diﬀerence in the four
transformed images (obtained by applying the above four filters on that image).

## 4. Histogram Equalization and Matching

(a) Perform histogram equalization of ‘selfie.jpg’. Save the histogram equalized image as ‘hist eq selfie.jpg’.
Display it and see how it diﬀers from ‘selfie.jpg’. Compare the histograms of ‘hist eq selfie.jpg’
and the original.

(b) Use cat image from the skimage.data package as the reference and match the histogram of
“selfie.jpg”. Plot the images and the corresponding histograms side by side and compare.
Now, use camera image as the reference and match the histogram of “selfie.jpg”. List your
observations.


# Image-Processing - 2

#### 1. A signal is provided in “signal 1.npy” file where the first column contains time index(in seconds) and the second column contains the amplitude of the signal.

(a) Load and plot the signal.

(b) Find the frequency components(in Hz) present in the signal and their magnitudes.

(c) From the above, write the expression for the continuous time signal from which the given signal
is sampled.

(d) What if we sample this (in part (c)) continuous time signal with 48 Hz? Plot the signal sampled
at 48 Hz. Reconstruct the signal using the sinc interpolation using the sampled signal.

(e) Based on your observation in part (d), choose a sampling frequency (as small as possible) so
that there is no aliasing.

(f) Add a phase shift of π/3 to all the sinusoidal components, i.e., sin(2πf t + π/3) you found in
part (c). Now, sample and reconstruct using 48 Hz. List your observations.

#### 2. Find the {8−, 32−, 128−} point DFT of the following signals and plot them (separately). Assume the sampling frequency is 10 Hz (i.e, x[n] is obtained by sampling a continuous signal x(t) with a sampling frequency 10 Hz), map the DFT coeﬃcients to actual frequencies and plot the magnitude spectrum.

(a) x[n] = {1↑, 1, 1, 1, 0, 0, 0, 0}.

(b) x[n] = {1↑, 0, 1, 0, 1, 0, 1, 0}.

#### 3. An image is provided in “image 1.npy”file which is generated by addition of scaled sine gratings of diﬀerent frequencies and phase angles.

(a) Load and plot the image.

(b) Find the DFT of the image and plot the magnitude and phase spectrum.

(c) What are the frequency components present in the image?

(d) Suppose the DFT of the image is denoted as Xf. The DC component of the image can be
removed by equating Xf[0, 0] = 0 and the modified DFT is denoted as X′f. Now, take the
inverse DFT of X′f and plot the resulting image. What do you observe?



















