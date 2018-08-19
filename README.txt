# pd-reactivision-wekinator
This pd patch extracts x,y and angle of a reacTIVision fiducial and sends it to Wekinator

This repository is located at https://github.com/teo523/pd-reactivision-wekinator

It contains a pd patch which extracts x,y, and angle of a reactivision fiducial and send these three features as an input to Wekinator (port 6448).

#INSTALLING INSTRUCTIONS:
Be sure on having last version of pd vanilla (I used pd-0.48).
You will need two libraries for this: 1)mrpeach and 2)TUIO

1) Download reacTIVision engine (for your specific OS) and reacTIVision TUIO Client for PureData, both available here --> http://reactivision.sourceforge.net/

You will have to tell pd where is located the TUIO folder. You can try with deken. If that doesn't work, you can manually add it with make command. Check this thread in forum where I found how to do it --> https://forum.pdpatchrepo.info/topic/11559/tuioclient-couldn-t-create

If you get "TUIO client couln't create", probably you have to create and save your pd patch within the same folder where TUIO is located. 


2) mrpeach is easily installed with deken: in pd go to the help tab -> search externals and search for mrpeach and click install.

#RUNNING IT
Just open the pd patch, reacTIVision, Wekinator listening on same port 6448 with 3 inputs and connect some of your choice output...and enjoy!

#THINGS TO TRY
You can connect the Processing_Drum_3ContinuousOutputs or other sound outputs available in http://www.wekinator.org/examples/ 
In this way, you can train wekinator to output specific sounds corresponding to specific locations of your fiducials. As an example, you can watch the video I made: https://www.youtube.com/watch?v=N9_Z0CjRdUE&feature=youtu.be
Also you can try to make a one to one correspondence from input to output, i.e., in Wekinator input window just toggle on the diagonal X's of the matrix. This would allow you to better explore each variable of your movements.
