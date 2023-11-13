# Blink-Counter-AI

Eye blink detection is one of the important problems in computer vision.

Before detecting blinks we need to detect the eyes. We will use the pre-trained facial landmark detector from Dlib to detect the 68 landmark points on the face. Then we will use the indexes of the eyes to extract the two eyes.

We will use the norm function from numpy to compute the euclidean distance between two points.

When we compute the aspect ratio, we will compare it with the threshold value. If the aspect ratio goes below the threshold and then rises above it, we will increment the blink counter.

Basically, what we are doing here is that we are checking if the eye aspect ratio goes below the blink threshold and then rises above it. If so, we count this as blinking so we increment the blink counter.

The final step is to draw the landmarks of the eyes, display the number of blinks, and the eye aspect ratio on the frame.
