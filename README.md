# RTFM
This repo contains the Pytorch implementation of our paper:
> [**Weakly-supervised Video Anomaly Detection with Robust Temporal Feature Magnitude Learning**](https://arxiv.org/pdf/2101.10030.pdf)
>
> [Yu Tian](https://yutianyt.com/), [Guansong Pang](https://sites.google.com/site/gspangsite/home?authuser=0), Yuanhong Chen, Rajvinder Singh, Johan W. Verjans, [Gustavo Carneiro](https://cs.adelaide.edu.au/~carneiro/).

- **Accepted at ICCV 2021.**  

- **SOTA on 4 benchmarks.** Check out [**Papers With Code**](https://paperswithcode.com/paper/weakly-supervised-video-anomaly-detection) for [**Video Anomaly Detection**](https://paperswithcode.com/task/anomaly-detection-in-surveillance-videos). 


## Training

### Setup

**Please download the extracted I3d features for ShanghaiTech and UCF-Crime dataset from links below:**

> [**ShanghaiTech train i3d onedirve**](https://uao365-my.sharepoint.com/:f:/g/personal/a1697106_adelaide_edu_au/EiLi_oBQnAFCq3UG184p_akB2sV7szCWvOV9PtaKJ6lxtQ?e=MeM3TE)
> 
> [**ShanghaiTech test i3d onedrive**](https://uao365-my.sharepoint.com/:f:/g/personal/a1697106_adelaide_edu_au/EvUUrWqpWqVHrXBzxbzAdD8BGiZBiumWWOaZmQ_AMAkAdg?e=P1rwCg)
> 
> [**ShanghaiTech train features on Google dirve**](https://drive.google.com/drive/folders/1z-CQPpVtTyfZyPKZdv2hZ-h2oMF6s8ep?usp=sharing)
> 
> [**ShanghaiTech test features on Google dirve**](https://drive.google.com/drive/folders/1L71Qa0gao6aLVhSjL0H-u2khmTRKcmQs?usp=sharing)


**Extracted I3d features for UCF-Crime dataset**

> [**UCF-Crime train i3d onedirve**](https://uao365-my.sharepoint.com/:f:/g/personal/a1697106_adelaide_edu_au/ErCr6bjDzzZPstgposv1ttYBudL8UVnap6eHS46fFbooAQ?e=RZsMtA)
> 
> [**UCF-Crime test i3d onedrive**](https://uao365-my.sharepoint.com/:f:/g/personal/a1697106_adelaide_edu_au/EsmBEpklrShEjTFOWTd5FooBVXbeoDHTTqPZn60Vj3Guhg?e=hvv46w)
> 
> [**UCF-Crime train I3d features on Google drive**](https://drive.google.com/drive/folders/1_6FVnHYpThVd2p93wjnbNs9g1ZuaUSTp?usp=sharing)
> 
> [**UCF-Crime test I3d features on Google drive**](https://drive.google.com/drive/folders/1QCBTDUMBXYU9PonPh1TWnRtpTKOX-fxr?usp=sharing)
> 
> [**checkpoint for Ucf-crime**](https://uao365-my.sharepoint.com/:u:/g/personal/a1697106_adelaide_edu_au/Ed0gS0RZ5hFMqVa8LxcO3sYBqFEmzMU5IsvvLWxioTatKw?e=qHEl5Z)


The following files need to be adapted in order to run the code on your own machine:
- Change the file paths to the download datasets above in `list/shanghai-i3d-test-10crop.list` and `list/shanghai-i3d-train-10crop.list`.
- Feel free to change the hyperparameters in `option.py`
### Train and test the RTFM
After the setup, simply run the following command: 
```shell
python main.py
```


## Citation

If you find this repo useful for your research, please consider citing our paper:

```bibtex
@inproceedings{tian2021weakly,
  title={Weakly-supervised Video Anomaly Detection with Robust Temporal Feature Magnitude Learning},
  author={Tian, Yu and Pang, Guansong and Chen, Yuanhong and Singh, Rajvinder and Verjans, Johan W and Carneiro, Gustavo},
  booktitle={Proceedings of the IEEE/CVF international conference on computer vision},
  year={2021}
}

```
---
