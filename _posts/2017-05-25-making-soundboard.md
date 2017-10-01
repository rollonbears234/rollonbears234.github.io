---
layout: post
title:  "Making a Soundboard"
date:   2017-05-25 19:45:31 +0530
categories: ["developer", "web"]
author: "Bryan Alcorn"
---

note: I chose not to include the pictures of the soundboard here in order to not embarrass my girlfriend, whose face is all over my soundboard.

### What is a soundboard

A soundboard is a collection of audio snippets that play when pressing an icon on a website. For my soundboard, I took all of the sounds I had recorded from videos with my girlfriend and I and I cut them to play embarrassing sounds she has made. I made it so that each sounds plays when an image of her is clicked on.

### Steps:

1. Download Soundflower: [Soundflower](https://github.com/mattingalls/Soundflower), you will need the soundflower bed and the tool to be installed. The bed lets you interact with soundflower and the normal tool just adds it to your sound system preferences and installs the features.

    * Follow this guide to configure correctly: [Macworld Guide to soundflower](http://www.macworld.com/article/1159440/software-graphics/soundflower-capture.html)
    * You will be using quicktime and Itunes or quicktime again to capture audio and play it to snip whatever audio you want to add to your soundboard.

2. Create your html and css website however you life. I made mine pretty simple with just a normal header. I used the following HTML snippet to add a picture and make a specific audio file play whenever it is clicked on.

    ```html
    <!DOCTYPE html>
    <html>

        <head>
            <title>This Soundboard!! </title>
            <link rel="stylesheet" type="text/css" href="mystyle.css">
        </head>
        <body>

            <h1>this Amazing Sounds</h1>

            <!-- First sound -->
            <audio id="sound1" src='./audio_clips/lonely_song.m4a' preload="auto"></audio>
            <a onclick="document.getElementById('sound1').play();">
                <img src="./Val_Headshots/grad_face.png">
            </a>
        </body>
    </html>
    ```

3. Keep repeating the picture and audio setup for as many audio clips you can find and want to add. The more audio, the more fun it is to click through and surprise yourself with random sounds. 

**Enjoy and make this with caution, it can be a fun way to embarrass a loved one.**
