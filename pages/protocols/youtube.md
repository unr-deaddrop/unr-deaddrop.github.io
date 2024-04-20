---
title: YouTube
layout: default
parent: Communication Protocols
---
## Description
This protocol uses YouTube's APIs and free video hosting service to tranfer data. Binary data is encoded as pixels in a video and published to the streaming site where it can be retrieved remotely and decoded. 

The data is encoded by taking each bit from the input data and writing an n x n square of pixels to
the output video with a white square corresponding to a binary 0 and a black square correlating to a
binary 1. The size of the square is configurable so that we can look into optimizing the
(de-)compression ratio and fighting YouTube’s compression algorithm that may corrupt
higher-density data streams.
