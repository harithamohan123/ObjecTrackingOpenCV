# Object Tracking Using OpenCV

Opencv :                                                                                                          
      OpenCV is a great tool to play with images and videos. Either you want to give your photos a 90s black and white look or perform complex mathematical operations OpenCV is always ready to serve.                                
      
 Object Tracking :                                                                                                                     
     Object tracking is the process of locating a moving object in a video.  dge of OpenCV is a must. The technique is widely used in surveillance, security, traffic monitoring, robot vision, video communication, and much more. Moreover, object tracking has several use cases such as crowd counting, self-driving cars, face detection, etc.                                                     
     
How to  run:                                                                                                                                  
     =>  First of all we import the required libraries that we will be using. (imutils and cv2)                                     
     =>  As you might know, videos are made of frames. Frames are nothing but one of many still images that together make up the whole moving picture. The next step will be reading those frames using the VideoCapture() function in OpenCV.                                                              
     =>  Use while loop to view the frames moving.                                                                                        
     =>  We will be defining a function that will resize the images so that they will fit on our screen in case they are big enough.                       
     =>  We are using the HSV colour format because it is more sensitive to minor changes in external lighting. Hence it will give more accurate masks and hence better results.                                                                                                                            
     =>  After converting the colourspace what we have to do is to filter out the red channel and create a mask frame.                          
     =>  findContours() which takes a masked image and returns an array of contours.                                                                
     =>  cv2.rectangle() function will draw the rectangle for us.                                                                                     
     =>  We will be using cv2.moments. cv2.moments calculates the weighted average sum of pixel intensities within the contour and hence allows to get some more useful information from the blob, like its radius, centroid, etc.                                                                                             
    =>  Adjust the speed of the video using cv2.waitKey(x) which pauses the screen for x milliseconds.                                                       
