---
title: OpenCV Installing and Getting Started on Raspberry Pi
description: >
  I have yet to be able to install OpenCV on a Raspberry PI.  Running
  out of SD card space was the killer, but there has to be a better
  way, let us go find one!
date: 2019-04-04
categories: 
  - opencv
  - software
  - computer vision
---


Install OpenCV on a raspberry pie, at least how I have been trying to
do it, by downloading the source code and building has been a very
tedious task, for which I have yet to celebrate any form of success.

## On to Plan B

Therefore I think I am going to head off and try plan B, for now Plan B is
one of the following three options:

1. Use PXE to boot The raspberry pie and mount the file systems over
   NFS.  I can then install OpenCV without concern for running out of
   space on the SD card.  In there the build should also go faster.
   
2. The second option would be simply to use raspberry pipe to stream
   the video from the raspberry pie to a another computer connected to
   the network that will then be able to process the streaming video.
   
3. A third option is to store the video locally and a later
   uploaded the video for post mobile processing. 
   
The third option is really not an option it is more of a feature that
required rather than a replacement for _Real Time_ OpenCV processing. 

Post process looses the _Real Time_ aspect of our camera and hence an
import requirement for the project.   But an important fallback
feature just the same.

## OpenCV on Linux VirtualBox

I am also manage some back up and install a open CV on my Mac
laptopWhich is becoming cluttered with a bunch nonsense, So I think I
will install open CD on a virtualMachine running clinicsAndy done with
it. 

I can use this to process Video Streams from a Raspberry Pi, at least
in theory.  But then if we can not do this, we are in really bad
shape! 

### Settle For OpenCV 2 on RPI

Well, as far as on vehicle processing, I am going to stick with
OpenCV-2 (ancient, OpenCV 4.0 recently released) but trying to build
was way to slow, so any software built on vehicle will have to be
constrained to OpenCV 2.0 for now.

Hopefully soon enough somebody will update the situation, which I
expect will be soon.

## Installed OpenCV 4.0.1 on VM

In the mean time, we can move our OpenCV 4.0 processing to a desktop
or VM for now.

To that end I compiled OpenCV straight from the github now ready to
go.

### Stream From RPI to Host?

We could go for streaming the video from the RPI to the host with
OpenCV 4.0 for advanced processing.  That sounds like something sexy
to do, but I wonder what the performance would be?

#### What about Performance?

Answer this question.
