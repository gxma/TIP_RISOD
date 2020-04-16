

### Pipeline

<img src="./pipeline.png" width=1200 height=200 />

### Requirements

- Linux
- Python 3.5+ ([Say goodbye to Python2](https://python3statement.org/))
- PyTorch 1.0+ or PyTorch-nightly
- CUDA 9.0+
- NCCL 2+
- GCC 4.9+
- [mmcv](https://github.com/open-mmlab/mmcv)

We have tested the following versions of OS and softwares:

- OS: Ubuntu 16.04/18.04 and CentOS 7.2
- CUDA: 9.0/9.2/10.0
- NCCL: 2.1.15/2.2.13/2.3.7/2.4.2
- GCC: 4.9/5.3/5.4/7.3

### Install mmdetection

1. Create a conda virtual environment and activate it. Then install Cython.

```shell
conda create -n mm python=3.7 -y
source activate mm

conda install cython
```

2. Install PyTorch stable or nightly and torchvision following the [official instructions](https://pytorch.org/).

3. Clone the mmdetection repository.

```shell
git clone https://github.com/open-mmlab/mmdetection.git
cd mmdetection
```
4. Compile cuda extensions.

```shell
./compile.sh
```

5. Install mmdetection (other dependencies will be installed automatically).

```shell
python setup.py develop
# or "pip install -e ."
```

6. RPN models are available in the [Model](https://github.com/NANSHANB/GARP/blob/master/MODEL_ZOO.md)

### Datasets and Results:

Dataset : [Drive Link](https://drive.google.com/open?id=1g60896zUp_HtQqAV28sAS5rEWrAR71aw) 

Results : [Drive Link(1cxf)](https://pan.baidu.com/s/1IniuvhnuGkvMTqIcbQAvlg)


### Usage

1. Please download our pretrained model at [Google Drive](https://drive.google.com/open?id=1GsS95QmhC0_WIuf-dhNHkMXbiMN4HwZd).   
   Put this model in `./models/` and `./reimg/`.

2. Run:

   ```shell
   main.m'
   ```
   
### Other Saliency Method

1. [EGNet](https://github.com/JXingZhao/EGNet/): EGNet:Edge Guidance Network for Salient Object Detection.

2. [BANet](http://cvteam.net/projects/ICCV19-SOD/BANet.html): Selectivity or Invariance: Boundary-aware Salient Object Detection.

3. [RFCN](https://pan.baidu.com/s/1XGhct3zvYIRKPafx2yAL-Q): Salient Object Detection with Recurrent Fully Convolutional Networks.

4. [RADF](https://github.com/xw-hu/RADF): Recurrently Aggregating Deep Features for Salient Object Detection.

5. [CPD](https://github.com/wuzhe71/CPD): Cascaded Partial Decoder for Fast and Accurate Salient Object Detection.

6. [BASNet](https://github.com/NathanUA/BASNet): BASNet: Boundary-Aware Salient Object Detection .

7. [PAGRN](https://github.com/zhangxiaoning666/PAGR): Progressive Attention Guided Recurrent Network for Salient Object Detection.

8. [MLMSNet](https://github.com/zhuxinang/MLMSNet): A Mutual Learning Method for Salient Object Detection with intertwined Multi-Supervision.

9. [PFA](https://github.com/CaitinZhao/cvpr2019_Pyramid-Feature-Attention-Network-for-Saliency-detection): Pyramid Feature Selective Network for Saliency detection.
   
### Useful Links

1. [DUTS-TR-5K](https://drive.google.com/open?id=1HhHftSK8FPSYTBKn1AcrXrx-4HAyqEv5): including 5000 training. The source images can be found [here](http://saliencydetection.net/duts/).

2. [DeepLearnToolbox](https://github.com/rasmusbergpalm/DeepLearnToolbox): Matlab/Octave toolbox for deep learning.

3. [Edges](https://github.com/pdollar/edges): Structured Edge Detection Toolbox.

4. [matconvnet](https://github.com/vlfeat/matconvnet): CNNs for MATLAB.

### Evaluation Method

Saliency Evaluation Method : The code for CRF can be found in [Ming-Ming Cheng](http://mmcheng.net) and [Deng-Ping Fan](http://dpfan.net/).

### Contacts
ma(###->@)jbeta(***->.)net
