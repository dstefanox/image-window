# image-window

`image-window` is aimed to be an alternative to `img` tag or `iron-image` component, allowing better control over image.
As its name says, concept of the component is to represent an image seen through the window. 

`image-window` is a hybrid component, so it can work with both polymer 1.x and 2.x.

**Window** is an rectangular transparent area in infinite non-transparent surface, and image is placed behind this surface.
Part of the image which is direcly below window is visible, while part of the image which is below non-transparent area is invisible.

Component allows resizing of the image in a various ways depending on a window size, as well as positioning of the resized image relative to window in a various ways.

For example, image can be scaled to fully fit into the window and to be centered on both axis.
Alignment and scaling can be changed dynamically and change from one state to another is animated.

## Live demo

To see live demo of the `image-window` element, visit element [demo page](http://dstefanox.github.io/image-window/components/image-window/)

## Installing

Install the component using [Bower](http://bower.io/):

```sh
$ bower install image-window --save
```

## Usage

### Import  Element:

```html
<link rel="import" href="bower_components/image-window/image-window.html">
```

### Place it on page:


Basic use case is practically the same as in case of `img` or `iron-image`. This shows image in its original size:

    <image-window src='test-image.jpg'></image-window>


Window may be defined by specifying `width` and `height` attributes of the component. Following will show :

    <image-window style='width:264px;height:264px;' src='test-image.jpg'></image-window>

The way in which image is resized relative to the window is defined using `fit` property of the `image-window`. Of course, size of the 'image-window' should be defined in order to make fit work as expected. In example below, image is resized to fit width of the window.

  	<image-window style='width:264px;height:264px;' src='test-image.jpg' fit='fitx'></image-window>
