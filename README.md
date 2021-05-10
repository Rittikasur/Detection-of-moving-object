# Detection-of-moving-object
Detection of moving objects in a video i.e. car, human, etc using opencv with 2 different methods.

1st Method - Median Filtering
This method is suitable for videos with fixed background.
Here the background is extracted using median filtering of 30 randomly extracted frames,this gives us the background of the video.
After having the background, we do a difference between each frame and the background to check for any moving object, if any found, a series of thresholding is done to extract the object and create a bounding box around the object.

2nd Method - Consecutive frame diffrence
Here 2 consecutive frames are captured and a difference between the frames, provides any kind of moving object.
Bounding box is drawn around the object detected.
