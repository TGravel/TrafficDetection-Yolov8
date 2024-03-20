# TrafficDetection-Yolov8
Transfer-learning a YoloV8 Model on the BDD-100K (10K) Detection Dataset.

Default YoloV8l Model | Our finetuned YoloV8l Model
:-: | :-:
<video src=https://github.com/TGravel/TrafficDetection-Yolov8/assets/36968003/36782b2c-198a-4e61-8845-592958277c91> | <video src=https://github.com/TGravel/TrafficDetection-Yolov8/assets/36968003/c6aa17dc-2902-4bed-ac2c-f9e5928c65d0>


## Startup Guide
### Requirements

- opencv-python>=4.6.0
- ultralytics>=8.1.29
- albumentations>=1.4.1
- torchvision>=10.2.0
- pytorch
- matplotlib
- tensorboard

If you use a PC with a NVDIA graphics card 
- install NVDIA Cuda>=12.1

#### Anaconda Installation

- open Anaconda Prompt.
- go to this github directory (requirements.txt)
- add conda-forge to channels

```
conda config --append channels conda-forge
```

- create new environment (if CUDA is installed)

```
conda create -n iav_assignment1 python>=3.7 pytorch-cuda=12.1 --file requirements.txt -c pytorch -c nvidia -y
```

- or for CPU only installation

```
conda create -n iav_assignment1 python>=3.7 --file requirements.txt -c pytorch -y
```

- this may take some time until all the packages are downloaded and installed
- run
 ```conda activate iav_assignment1 ``` after the installation is complete
- if everything was installed successfully you should be able to start the notebook using `jupyter notebook` and see your graphics card (cpu) as used device.
- set notebook as trusted to view videos!
- training the model and can be enabled via the constants defined in the notebook

#### Remove environment
- Use `conda remove -n iav_assignment1 --all` to delete the environment after use.

### Run:
- set constants to decide what parts of the notebook you want to execute
- run the jupyter notebook

### Source:
- bdd100k (https://www.vis.xyz/bdd100k/)
- yolov8 (https://github.com/ultralytics/ultralytics)

### Contact
- if there is any problem running this code, please contact: Nico.hanner@gmx.at


