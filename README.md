This is a modified version of the code behind the 
[Switching Eds blog post](http://matthewearl.github.io/2015/07/28/switching-eds-with-python/).
This version runs in real time on a camera input.

See the link for an explanation of the code.

To run the script you'll need to install dlib (http://dlib.net) including its
Python bindings, and OpenCV. You'll also need to obtain the trained model [from
sourceforge](http://sourceforge.net/projects/dclib/files/dlib/v18.10/shape_predictor_68_face_landmarks.dat.bz2).

Unzip with `bunzip2` and change `PREDICTOR_PATH` to refer to this file. The
script is run like so:

    ./faceswap.py <face image> 

If successful, the facial features of the first face detected in the
input video will be replaced with the facial features from `<face image>`
and displayed live in the output window.

