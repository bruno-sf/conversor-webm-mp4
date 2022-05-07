# conversor-webm-mp4
An Alpine based docker image to convert webm to mp4 without having to install ffmpeg locally which in my case is conflicting with AMD VideoCard Libs

Link:https://hub.docker.com/repository/docker/brunoferreira/conversor-webm-mp4


Why ``this``?
-----------------------
I've been using for a time a bash alias with some useful command using the ffmpeg for converting media files.
After updating my videocard ATI/AMD I discover a pretty annoying bug that messup with my ffmpeg, after a workaround using an isolated ffmpeg instalation at /home/$USER/ffmpeg, I decide to move change my alias to something more clean using Docker. TLDR: Docker to the rescue!

![error](https://imgur.com/jDYxnTG.png)


### Prerequisites

- Docker 🐋

### Usage

The usage is pretty forward, just pass the directory with the videos you want to convert using *-v* argument.

```
docker run -it -v ${HOME}/Downloads/:/conversor conversor-webm-mp4
```

![run](https://imgur.com/1EnFuTZ.png)

### TODO and Thoughts :thought_balloon:
TODO.

- [  ] - More options with ffmpeg using arguments

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
