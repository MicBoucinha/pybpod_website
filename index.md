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
  - image_path: /assets/images/generate_sound2.png
    alt: "placeholder image 1"
    title: "Uuuhh so pretty"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: /assets/images/generate_sound2.png
    alt: "placeholder image 2"
    title: "Documentation"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: /assets/images/generate_sound2.png
    title: "Plugins"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."

---

# Bpod State Machine #
![image-right](/assets/images/bpod.jpg){: .align-right}
Bpod is a system from [Sanworks](https://sanworks.io){:target="_blank"} for precise measurement of small animal behavior. It is a family of open source hardware devices which includes also software and firmware to control these devices. The software was originally developed in MATLAB providing retro-compatibility with the BControl system.

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
