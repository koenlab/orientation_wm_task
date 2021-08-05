# Teardrop Orientation Working Memory Task

This is the orientation task reported by Bae and Luck (2018) in the Journal of Neuroscience. 

Briefly, an angle of 0 degrees corresponds to the point of the teardrop pointing to the right on the x-axis. Positive angles start to tilt the teardrop _down_ (i.e., a negative y-axis value) whereas negative angles tilt the teardrop _up_ (i.e., positive y-values). In line with this, angles between +90 (i.e., point (0, -1) here) and +270 (i.e., point (0, 1) here) have negative x-coordinate values for the point of the teardrop. 

TO-DO: Add some example images to show this. 

Some other notes:
- Errors are cacluated from -180 to + 180 (following the same convention described above)
- Currently, the task adds +/- 5 degrees of 'error' to the target angle to avoid some categorical coding. 
- The timing slightly differs from that of Bae and Luck in that there is a slightly longer period between trials (i.e., end of the test response, beginning of the next encoding probe), and some of this is filled with a fixation cross. 
- The mouse cursor is hidden just after the test probe appears, and is auto-set to a random location on the circle. 
- Options for the task can be (mainly) controlled with the code component in the config routine. This includes timing, teardrop length/size, the range of error added to the angle bins, etc. 
- To change the center of the angle bins (or the bins overall), modifiy the angle_conditions.csv file
- Unlike Bae and Luck, this task does not use 0 as one of the angles. All angles are offset by 12.25 degrees from 0 (compared to what Bae and Luck used) to avoid orientations that lie along the abscissa and ordinate. 