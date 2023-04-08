# GMFSS_Fortuna
The All-In-One GMFSS: Dedicated for Anime Video Frame Interpolation, based on https://github.com/98mxr/GMFSS_Fortuna.


## Dependencies
- [CuPy](https://docs.cupy.dev/en/stable/install.html)
- [NumPy](https://numpy.org/install)
- [PyTorch](https://pytorch.org/get-started) 1.13.1
- [VapourSynth](http://www.vapoursynth.com/) R55+

`trt` requires additional runtime libraries:
- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) 11.7
- [cuDNN](https://developer.nvidia.com/cudnn) 8.6
- [TensorRT](https://developer.nvidia.com/tensorrt) 8.6.0.12

For ease of installation on Windows, you can download the 7z file on [Releases](https://github.com/HolyWu/vs-gmfss_fortuna/releases) which contains required runtime libraries and Python wheel file. Unzip the file to the location that you chose. Add `<unzippath>/bin` to your system `PATH`. Additionally, add `<unzippath>` to `CUDA_PATH` environment variable because CuPy relies on it. Finally pip install the Python wheel file.


## Installation
```
pip install -U vsgmfss-fortuna
```


## Usage
```python
from vsgmfss_fortuna import gmfss_fortuna

ret = gmfss_fortuna(clip)
```

See `__init__.py` for the description of the parameters.
