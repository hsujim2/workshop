## Environment
Windows 11 insider preview build 22598<br>
Ubuntu 22.04 with WSL2 and WSLg enabled<br>
CPU:I5-12400<br>
GPU:RTX-3070<br>

## install WSL
Download Ubuntu 22.04 and windows terminal(some are inbuilt) in windows store.<br>
Open windows terminal.<br>
>wsl --install<br>

Open ubuntu, ubuntu 22.04 LTS with WSLg have graphical setup.<br>
![Imgur](https://i.imgur.com/CLSfoHE.png)
![Imgur](https://i.imgur.com/jEDm2rt.png)
![Imgur](https://i.imgur.com/AtunTSC.png)
![Imgur](https://i.imgur.com/Vp0n0GO.png)
![Imgur](https://i.imgur.com/cUmou9t.png)
![Imgur](https://i.imgur.com/AE14hNH.png)

## install environment
>sudo apt install python3-pip nvidia-driver-510 nvidia-dkms-510 unzip zip<br>
>nvidia-smi<br>

![Imgur](https://i.imgur.com/urIU9Ty.png)
>pip3 install keras_unet_collection numpy opencv-python matplotlib tensorflow-gpu keras<br>

Prepare predict_multiple_image.py, predict.zip and segmentation_model_weight.hdf5 three files.<br>
![Imgur](https://i.imgur.com/1WMige0.png)
Change path in predict_multiple_image.py.<br>
>python3 predict_multiple_image.py<br>

## Automatically convert NIFTI to IMAGE file
>pip3 install -r requirement.txt<br>

Change path in tii2image.py.<br>
>python3 tii2image.py<br>
