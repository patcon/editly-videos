# Demo: Editly with GitHub Actions

[![Make Video](https://github.com/patcon/editly-videos/workflows/Make%20Video/badge.svg)](https://github.com/patcon/editly-videos/actions?query=workflow%3A%22Make+Video%22)

![GIF from generated release asset](https://github.com/patcon/editly-videos/releases/latest/download/editly-demo-video.gif)

An exploration of _Continuous Video Production_ for open source projects.

This repo is for exploring how GitHub Actions might be used to conveniently and iteratively manage the creation of promotional and support videos for open source projects.
We do this with a version-controlled "director" file, which generated the video using **Editly**, a video editing API and command-line tool.

What's here:
- `inputs/my-video.json5`: The director video config file.
- `.github/workflows/make-video.yml`: The GitHub Actions workflow files run on every commit.
- [Sample GitHub Actions build page][build-page]: A successful build, where stored video is saved.

   [build-page]: https://github.com/patcon/editly-videos/actions/runs/407859315
   
![screenshot of build page with artifact](docs/build-page.png)

## Tools Used

- [Editly](https://github.com/mifi/editly)
  - `ffmpeg` under the hood
- GitHub Actions
- Docker Compose

## See Also

- https://github.com/mifi/editly/pull/96
- https://github.com/pol-is/polis/issues/130
