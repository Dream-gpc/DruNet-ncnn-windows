# DRUNet-ncnn-windows
This is an unofficial simple implementation of DRUNet based on ncnn.


## 环境准备
* Visual studio 2019/2022  
* NCNN 你可以在此处[下载](https://github.com/Tencent/ncnn/releases)ncnn预编译版本  
* Opencv 4.6.0  


## 使用方式
编译成功后使用以下命令即可  

`./<xxx.exe>  <image-path>` 


## 结果

### 灰度图

* Gray 25:  

| Input | Pytorch | ncnn |
| --- | --- | --- |
|  <img src="https://github.com/Dream-gpc/DeamNet-ncnn-windows/blob/main/imtest/noiseimg1.png" width="300px">   | <img src="https://github.com/Dream-gpc/DeamNet-ncnn-windows/blob/main/results/denoiseimg1.png" width="300px"> | <img src="https://github.com/Dream-gpc/DeamNet-ncnn-windows/blob/main/results/denoiseimg1-ncnn.png" width="300px"> | 
|  <img src="https://github.com/Dream-gpc/DeamNet-ncnn-windows/blob/main/imtest/noiseimg2.png" width="300px"> | <img src="https://github.com/Dream-gpc/DeamNet-ncnn-windows/blob/main/results/denoiseimg2.png" width="300px"> |  <img src="https://github.com/Dream-gpc/DeamNet-ncnn-windows/blob/main/results/denoiseimg2-ncnn.png" width="300px"> | 


### 彩色图

| Input | Pytorch | ncnn |
| --- | --- | --- |
|  <img src="https://github.com/Dream-gpc/DeamNet-ncnn-windows/blob/main/imtest/cnoiseimg1.jpg" width="300px">   | <img src="https://github.com/Dream-gpc/DeamNet-ncnn-windows/blob/main/results/cdenoiseimg1.jpg" width="300px"> | <img src="https://github.com/Dream-gpc/DeamNet-ncnn-windows/blob/main/results/cdenoiseimg1-ncnn.png" width="300px"> | 

## Runtime

在AMD Ryzen 5 5600G上进行测试  


| 分辨率 | CPU | 核显+vulkan | 独显+vulkan:sob:|
| --- | --- | --- | --- | 
| 256x256 | --- | 2.62 | --- | 
| 1200x1600 | --- | 19.73 | --- | 

## Citation
> 
    @article{zhang2021plug, % DPIR & DRUNet & IRCNN
    title={Plug-and-Play Image Restoration with Deep Denoiser Prior},
    author={Zhang, Kai and Li, Yawei and Zuo, Wangmeng and Zhang, Lei and Van Gool, Luc and Timofte, Radu},
    journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
    year={2021}
    }


## License
[MIT © Dream-gpc](https://github.com/Dream-gpc/DruNet-ncnn-windows/blob/main/LICENSE)


修订中:relaxed:………………………………


