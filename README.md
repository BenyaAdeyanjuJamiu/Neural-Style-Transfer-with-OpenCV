# Neural-Style-Transfer-with-OpenCV
Neural Style Transfer with OpenCV  with a simple explanation and few lines of Codes
The original neural style transfer algorithm was introduced by Gatys et al. in their 2015 paper, 
A Neural Algorithm of Artistic Style
In 2016, Johnson et al. published Perceptual Losses for Real-Time Style Transfer and Super- Resolution,
which frames neural style transfer as a super-resolution-like problem using perceptual loss. 
The end result is a neural style transfer algorithm which is up to three orders of magnitude faster than the Gatys et al. 
method 
You can learn how to apply the neural style transfer algorithm to your own images and video streams.

To learn how to apply neural style transfer using OpenCV and Python, just keep reading!

    ********What is neural style transfer?****
    Neural style transfer is the process of:

    1) Taking the style of one image
    2) And then applying it to the content of another image
    
    **********How does neural style transfer work?*********
    Interestingly, the original 2015 paper by Gatys et al. proposed a neural style transfer algorithm that does not
    require a new architecture at all. Instead, we can take a pre-trained network (typically on ImageNet) and define a
    loss function that will enable us to achieve our end goal of style transfer and then optimize over that loss function.
    
    
    ***Therefore, the question isn’t “What neural network do we use?” but rather “What loss function do we use?”***

      The answer is a three-component loss function, including:

       1) Content loss
       2) Style loss
       3) Total-variation loss
       
 Each component is individually computed and then combined in a single meta-loss function. By minimizing the meta-loss function
 we will be in turn jointly optimizing the content, style, and total-variation loss as well.
 
 While the Gatys et al. method produced beautiful neural style transfer results, the problem was that it was quite slow.
 
 
 Johnson et al. (2016) built on the work of Gatys et al., proposing a neural style transfer algorithm that is up to
 three orders of magnitude faster. The Johnson et al. method frames neural style transfer as a super-resolution-like 
 problem based on perceptual loss functions
 
 
 Johnson et al. provide documentation on how to train your own neural style transfer models
  on their official GitHub page.
  
  Finally, it’s also worth noting that that in Ulyanov et al.’s 2017 publication, Instance Normalization: 
  The Missing Ingredient for Fast Stylization, it was found that swapping batch normalization for instance normalization 
  (and applying instance normalization at both training and testing), leads to even faster real-time performance and
  arguably more aesthetically pleasing results as well
  
  You can see the code ,try it and use any images you wish and you can use the real-time video or WebCam

