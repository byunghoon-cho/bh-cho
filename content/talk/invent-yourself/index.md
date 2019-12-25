+++
title = "Mechanical Random Number Generator"
date = 2016-06-28T17:00:00
#date_end = 2030-06-01T15:00:00
all_day = false

# Schedule page publish date (NOT talk date).
draft = false
publishDate = 2019-03-12T20:30:00

authors = ["bh"]

# Name of event and optional event URL.
event = "International Young Physicists' Tournament 2016"
event_url = "https://iypt.urfu.ru/en/"
location = "Yekaterinburg, Russia"

abstract = "Built a mechanical pseudo random number generator. Numbers generated were tested for randomness and tampering with statistics."
#summary = ""

featured = true
projects = []
tags = ["Physics", "C++", "Statistics"]

slides = ""

url_pdf = ""
url_slides = "slides/invent-yourself.pdf"
url_video = ""
url_code = ""

math = true

[image]
    caption = "Schematics of the random number generator"

    # Focal point (optional)
    # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
    focal_point = "Center"
+++

Random numbers are extremely difficult to generate. This project focused on designing a *mechanical* random number generator (RNG) as well as statistically analysing both the degree of randomness and the ability to detect tampering.

The webcam shown in the schematics was connected to my computer, running a program I wrote in C++ using the [OpenCV](https://opencv.org) library. Every 500 milliseconds, the colour of the highest, leftmost ball was recorded with empty frames disregarded. The colour is recorded in binary, 0 coding for red and 1 for green. Taking a certain number of bits allows the generation of larger numbers. For example, taking three bits of data gives numbers between 0 (000) and 7 (111).

Several methods of tampering were considered, including:

* Altering lighting conditions to change what colour balls the camera sees
* Changing the shape of the balls
* Changing the mass of the balls
* Removing a number of balls of one colour
* Changing the total number of balls in the RNG

This project was originally presented at the 2016 [International Young Physicists' Tournament](http://iypt.org/Home). The problem was:

> Truly random numbers are a very valuable and rare resource. Design, produce, and test a mechanical device for producing random numbers. Analyse to what extent the randomness produced is safe against tampering

{{% alert note %}}
The slides presented are available at the top of this page.
{{% /alert %}}
