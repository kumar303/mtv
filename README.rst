``mtv.py`` is a script that turns an mp3 file and an image file into a video.

You know what used to be cool? MTV. Music on TV.
I'm actually pretty excited that YouTube is turning
into a platform for sharing and discovering music.
They figured out the embedding part, the API part, and
they even figured out how to automatically pay rights holders
through digital fingerprinting.

``mtv.py`` is a script that anyone can easily use
if they have basic command line savvy to turn an mp3
+ image into a video file that can be uploaded to YouTube.
The video will show the image continuously while the song
plays, that's it.

Installation
------------

If you're on Mac or Linux this is going to be a breeze.
Read `this <http://ruby.about.com/od/tutorials/ss/commandline.htm>`_
if you've never used the command line before. It's easy.
If you're on Windows it will be easy too but you may need to
set up some paths and read some online tutorials.

Get `ffmpeg`_. If you're on a Mac and you have `homebrew`_
then type this to install it::

    brew install ffmpeg

On Linux (Ubuntu) type::

    sudo apt-get install ffmpeg

Clone this repo to your home directory (or wherever)::

    git clone https://github.com/kumar303/mtv.git ~/mtv

If you don't have the `git`_ command then
download the `zip <https://github.com/kumar303/mtv/archive/master.zip>`_
file, unzip it to your home dir, and make sure the
script is executable::

    chmod +x ~/mtv/mtv.py

Test it by changing into the directory of the code
and passing the help flag to see the usage::

    cd ~/mtv
    ./mtv.py --help

Usage
-----

One you have an mp3 file and an image you want to
turn into a video, just run something like this::

    ./mtv.py --song /path/to/song.mp3 --art /path/to/cover.jpg

You can then upload the ``mtv.mpg`` file to YouTube.

You don't have to use an mp3 file, you can use any audio
file that `ffmpeg`_ supports which is pretty much every
audio file.

.. _ffmpeg: http://ffmpeg.org/
.. _homebrew: http://mxcl.github.com/homebrew/
.. _git: http://git-scm.com/
