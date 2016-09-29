This is an experiment which combines the Depth Image captured from a Kinect Sensor with a Convolutional Neural Network, made for the purpose of recreating artistic styles of paintings. 

The folder contains a [Processing code](https://github.com/krohak/Projects/blob/master/Kinect/DepthImage_CNN/simple_depth_image/simple_depth_image.pde) for displaying the Depth Image and RGB Image from the Kinect sensor. 
Modified version of the code taken from the book [Making Things See](http://makingthingssee.com/) by  [Greg Boreinstein](http://gregborenstein.com/). Works on [Processing v2.2.1](https://processing.org/download/?processing). 

### Output
<img src="https://raw.githubusercontent.com/krohak/Projects/master/Kinect/DepthImage_CNN/simple_depth_image/Capture.PNG" width="500px">

This image is then passed onto a [Torch implementation](https://github.com/jcjohnson/neural-style) of the paper [A Neural Algorithm of Artistic Style](http://arxiv.org/abs/1508.06576) (Leon A. Gatys, Alexander S. Ecker, and Matthias Bethge) by [Justin Johnson](http://cs.stanford.edu/people/jcjohns/). 
The procedure of installing the dependencies is elaborated on [here](https://github.com/jcjohnson/neural-style/blob/master/INSTALL.md). I decided to use Torch 7 on Arch Linux, with optimization using ADAM and CPU mode (as explained by Justin Johnson) , since I have a low-end GPU. 