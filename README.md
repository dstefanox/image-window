# image-window

`image-window` is aimed to be an alternative to `img` tag or `iron-image` component, allowing better control over image.
As its name says, concept of the component is to represent an image seen through the window. 

**Window** is an rectangular transparent area in infinite non-transparent surface, and image is placed behind this surface.
Part of the image which is direcly below window is visible, while part of the image which is below non-transparent area is invisible.

Component allows resizing of the image in a various ways depending on a window size, as well as positioning of the resized image relative to window in a various ways.

For example, image can be scaled to fully fit into the window and to be centered on both axis.
Alignment and scaling can be changed dynamically and change from one state to another is animated.

## Installing

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install


## Usage

Basic use case is practically the same as in case of `img` or `iron-image`. This shows image in its original size:

    <image-window src='test-image.jpg'></image-window>


Window may be defined by specifying `width` and `height` attributes of the component. Following will show :

    <image-window style='width:264px;height:264px;' src='test-image.jpg'></image-window>
