---
layout: page
title: GooFit
tagline: A RooFit like fitter for GPUs and OpenMP
description: Home page for GooFit
---

## The package

GooFit is a powerful, fast fitting library designed to mimic the familar syntax of [ROOT](https://root.cern.ch)'s RooFit. The code and installation instructions are [available on GitHub](https://github.com/GooFit/GooFit), and a description of the fitting process and API is available on [GitHub IO](https://GooFit.github.io/GooFit).


## Docker builds

The development version of GooFit is available through Docker as well. To use the OpenMP version:


~~~bash
docker run -it goofit/goofit-omp
~~~

And, the CUDA version:

~~~bash
nvidia-docker run -it goofit/goofit-cuda
~~~

This will put you in a `/GooFit` folder. You should git pull the latest changes, and then go to `/GooFit/build` and rebuild. If you have a GooFit Package, you can check it out to `/GooFit/goofit_*`. If you want to persist you session, you should use Docker to mount a volume or folder.

The source for the docker builds is [available on GitHub](https://github.com/GooFit/docker-goofit).

## Acknowledgement 

GooFit's development has been supported by the National Science Foundation under grant number NSF-1005530. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the developers and do not necessarily reflect the views of the National Science Foundation.
