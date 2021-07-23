The preprocessing pipeline is the following:

Gregwchase approach

 Crop images into 1800x1800 resolution
 Resize images to 512x512/256x256 resolution
 Remove totally black images form dataset
 Rotate and mirror(Rotate DR images to 90°,120°,180°,270° + mirror, and only mirror non-DR images)
 Update CSV so it should contain all the augmented images and there respective labels
 Convert images to numpy array
 
Ms.Sheetal Maruti Chougule/Prof.A.L.Renke approach

 Image Denoising
 CLAHE (Contrast Limited Adaptive Histogram Equalization)
 
Ben Graham approach (*Only Works in python2.7)

 Rescale the images to have the same radius (300 pixels or 500 pixels)
 Subtracted the local average color; the local average gets mapped to 50% gray
 Clipped the images to 90% size to remove the boundary effects
