---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: splash
title: PyBpod
excerpt: Real-time behaviour measurement software
header:
    overlay_color: "#333"
    overlay_image: /assets/images/pybpod2.png
feature_row:
  - image_path: /assets/images/pypi.svg
    alt: "placeholder image 1"
    title: "Available in PyPI"
    excerpt: |
      Available through Python Package Index (PyPI) with ``` pip install pybpod ```  

      More detailed installation instructions on the [Installing and updating](https://pybpod.readthedocs.io/en/v1.7.8/getting-started/install.html){:target="_blank"} <i class="fas fa-external-link-alt fa-xs"/> section of the documentation.
    alt: "placeholder image 2"
    title: "Documentation"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: /assets/images/generate_sound2.png
    title: "Plugins"
    excerpt: "Extensibility through plugins. Please see the Plugins page for a list of available plugins.\n\nInstructions to guide you to start developing your own plugins are available in the documentation"

---
{% capture notice-text %}
* [Bpod device](https://sanworks.io/shop/viewproduct?productID=1024){:target="_blank"} {% include external-link.html %}
* [Bpod on Github](https://github.com/sanworks/Bpod){:target="_blank"} {% include external-link.html %}
* [Bpod Wiki](https://sites.google.com/site/bpoddocumentation/){:target="_blank"} {% include external-link.html %}
* [BControl project](http://brodywiki.princeton.edu/bcontrol/index.php/Main_Page/){:target="_blank"} {% include external-link.html %}
{% endcapture %}

![bpod state machine](/assets/images/bpod.jpg){: .align-right}
# Bpod #
Bpod is a system from [Sanworks](https://sanworks.io){:target="_blank"} {% include external-link.html %} for precise measurement of small animal behaviour. It is a family of open source hardware devices which includes also software and firmware to control these devices. The Bpod State Machine can connect to different modules
such as a Valve Driver, Analog Input, Analog Output, an Optical Lickmeter, among others. More information regarding available modules can be found at [Sanworks Store website](https://sanworks.io/shop/products.php?productFamily=bpod){:target="_blank"} {% include external-link.html %}.

The software was originally developed in MATLAB providing retro-compatibility with the BControl system.

<div class="notice--info">
  <h4>For further information please check the following links</h4>
  {{ notice-text | markdownify }}
</div>

{% include feature_row id="intro" type="center" %}

![Python logo](/assets/images/Python-logo-notext.svg){: .align-right}
# PyBpod #
PyBpod is a Python port of the [Bpod Matlab project](https://github.com/sanworks/Bpod>){:target="_blank"} {% include external-link.html %}. It is a GUI application that enables interaction with the latest [Bpod devices](https://sanworks.io/shop/products.php?productFamily=bpod){:target="_blank"} {% include external-link.html %}.

This project is maintained by a team of software developers at the [Champalimaud Foundation](http://research.fchampalimaud.org){:target="_blank"} {% include external-link.html %}.

<!-- <i class="fa fa-camera-retro fa-5x"></i>  <i class="fa fa-book fa-5x"></i> 

wee

![python-logo](/assets/images/Python-logo-notext.svg) <i class="fab fa-python fa-5x"></i> 

weeeee -->

{% include feature_row id="intro" type="center" %}

{% include feature_row %}


{% highlight python linenos %}
def my_softcode_handler(data):
    global start, soundStream, timeit, cam, camOK
    print(data)
    if data == 55:
        print("----PLAY-----")
        soundStream.playSound()
        start = timeit.default_timer()
        if not camOK:
            cam.record()
            camOK = True
    elif data == 66:
        soundStream.stopSound()
        print(':::::::::Time to stop:::::::::', timeit.default_timer() - start)
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}


Testing elements:

# Temporary information #
Nam elementum nisl et mi a commodo porttitor. Morbi sit amet nisl eu arcu faucibus hendrerit vel a risus. Nam a orci mi, elementum ac arcu sit amet, fermentum pellentesque et purus. Integer maximus varius lorem, sed convallis diam accumsan sed. Etiam porttitor placerat sapien, sed eleifend a enim pulvinar faucibus semper quis ut arcu. Ut non nisl a mollis est efficitur vestibulum. Integer eget purus nec nulla mattis et accumsan ut magna libero. Morbi auctor iaculis porttitor. Sed ut magna ac risus et hendrerit scelerisque. Praesent eleifend lacus in lectus aliquam porta. Cras eu ornare dui curabitur lacinia.

Nam elementum nisl et mi a commodo porttitor. Morbi sit amet nisl eu arcu faucibus hendrerit vel a risus. Nam a orci mi, elementum ac arcu sit amet, fermentum pellentesque et purus. Integer maximus varius lorem, sed convallis diam accumsan sed. Etiam porttitor placerat sapien, sed eleifend a enim pulvinar faucibus semper quis ut arcu. Ut non nisl a mollis est efficitur vestibulum. Integer eget purus nec nulla mattis et accumsan ut magna libero. Morbi auctor iaculis porttitor. Sed ut magna ac risus et hendrerit scelerisque. Praesent eleifend lacus in lectus aliquam porta. Cras eu ornare dui curabitur lacinia.

{% include video id="XsxDH4HcOWA" provider="youtube" %}

Nam elementum nisl et mi a commodo porttitor. Morbi sit amet nisl eu arcu faucibus hendrerit vel a risus. Nam a orci mi, elementum ac arcu sit amet, fermentum pellentesque et purus. Integer maximus varius lorem, sed convallis diam accumsan sed. Etiam porttitor placerat sapien, sed eleifend a enim pulvinar faucibus semper quis ut arcu. Ut non nisl a mollis est efficitur vestibulum. Integer eget purus nec nulla mattis et accumsan ut magna libero. Morbi auctor iaculis porttitor. Sed ut magna ac risus et hendrerit scelerisque. Praesent eleifend lacus in lectus aliquam porta. Cras eu ornare dui curabitur lacinia.

Nam elementum nisl et mi a commodo porttitor. Morbi sit amet nisl eu arcu faucibus hendrerit vel a risus. Nam a orci mi, elementum ac arcu sit amet, fermentum pellentesque et purus. Integer maximus varius lorem, sed convallis diam accumsan sed. Etiam porttitor placerat sapien, sed eleifend a enim pulvinar faucibus semper quis ut arcu. Ut non nisl a mollis est efficitur vestibulum. Integer eget purus nec nulla mattis et accumsan ut magna libero. Morbi auctor iaculis porttitor. Sed ut magna ac risus et hendrerit scelerisque. Praesent eleifend lacus in lectus aliquam porta. Cras eu ornare dui curabitur lacinia.

Nam elementum nisl et mi a commodo porttitor. Morbi sit amet nisl eu arcu faucibus hendrerit vel a risus. Nam a orci mi, elementum ac arcu sit amet, fermentum pellentesque et purus. Integer maximus varius lorem, sed convallis diam accumsan sed. Etiam porttitor placerat sapien, sed eleifend a enim pulvinar faucibus semper quis ut arcu. Ut non nisl a mollis est efficitur vestibulum. Integer eget purus nec nulla mattis et accumsan ut magna libero. Morbi auctor iaculis porttitor. Sed ut magna ac risus et hendrerit scelerisque. Praesent eleifend lacus in lectus aliquam porta. Cras eu ornare dui curabitur lacinia.

Nam elementum nisl et mi a commodo porttitor. Morbi sit amet nisl eu arcu faucibus hendrerit vel a risus. Nam a orci mi, elementum ac arcu sit amet, fermentum pellentesque et purus. Integer maximus varius lorem, sed convallis diam accumsan sed. Etiam porttitor placerat sapien, sed eleifend a enim pulvinar faucibus semper quis ut arcu. Ut non nisl a mollis est efficitur vestibulum. Integer eget purus nec nulla mattis et accumsan ut magna libero. Morbi auctor iaculis porttitor. Sed ut magna ac risus et hendrerit scelerisque. Praesent eleifend lacus in lectus aliquam porta. Cras eu ornare dui curabitur lacinia.


# Documentation #
For further information, please check the PyBpod's Read the Docs page at [https://pybpod.readthedocs.io](https://pybpod.readthedocs.io){:target="_blank"} 
