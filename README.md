# BilinearImageResize
Bilinear Image Resize with openmp/cuda<br />

Requirements:

>CUDA driver<br />
docker + nvidia docker

## Building:<br />

```bash
git clone http://github.com/royinx/BilinearImageResize

docker build -t opencv_trt .
docker run --rm -it --runtime=nvidia -v ${PWD}:/workdir -w /workdir opencv_trt bash

# inside container
mkdir build
cd build
cmake ..
clear && make && ./example
```