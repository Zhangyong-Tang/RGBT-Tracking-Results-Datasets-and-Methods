## RGBT-Tracking-Results-Datasets-and-Methods

**An investigation for RGBT tracking. 
Hopefully, it can help other researchers become familiar with multi-modal tracking as soon as possible.
This repository is started on 02/07/2023, and will keep on updating.**

-----
>This repository will give a detail investigation of the RGBT tracking community, including the Datasets, Results, and the Methods.
> 
>  - [x] Datasets
>  - [x] Results
>  - [x] Methods
>  - [x] Competitions
>  -  ...
-----

## Survey Papers
* Multi-modal visual tracking: Review and experimental comparison. Zhang, Pengyu, Dong Wang*, and Huchuan Lu. Computational Visual Media 2024. [[Paper](https://link.springer.com/article/10.1007/s41095-023-0345-5)]
* RGBT tracking: A comprehensive review. Mingzheng Feng, Jianbo Su*. Information Fusion 2024. [[Paper](https://www.sciencedirect.com/science/article/pii/S1566253524002707)]
* Review and Analysis of RGBT Single Object Tracking Methods: A Fusion Perspective. Zhihao Zhang, Jun Wang, Zhuli Zang, Lei Jin, Shengjie Li, Hao Wu*,Jian Zhao, Zhang Bo. ACM TOMM 2024. [[Paper](https://dl.acm.org/doi/10.1145/3651308)]
* Object fusion tracking based on visible and infrared images: A comprehensive review. Xingchen Zhang, Ping Ye, Henry Leung, Ke Gong, Gang Xiao*. Information Fusion 2020. [[Paper](https://www.sciencedirect.com/science/article/pii/S1566253520302657)]
* A Survey for Deep RGBT Tracking. Zhangyong Tang, Tianyang Xu, and Xiao-Jun Wu*. Arxiv 2022. [[Paper](https://arxiv.org/abs/2201.09296)]


## Datasets
***Real Data***

| Dataset | Publish  | GitHub| Introduction|
|--|--|--| --|
| OTCBVS | CVIU'2007 | [OTCBVS](http://vcipl-okstate.org/pbvs/bench/) | 9 videos|
| LITIV | CVIU'2012 | [LITIV](https://www.polymtl.ca/litiv/en/codes-and-datasets) | 6 videos|
| GTOT | TIP'2016 | [GTOT](https://pan.baidu.com/s/1QNidEo-HepRaS6OIZr7-Cw) | 50 Video pairs, about 1.5W frames|
| RGBT210| ACM MM'2017 | [RGBT210](https://drive.google.com/file/d/0B3i2rdXLNbdUTkhsLVRwcTBTMlU/view?resourcekey=0-vytg_w3hqlQfLhoiS2J8Dg) | 210 Video pairs|
| RGBT234| PR'2018 | [RGBT234](https://sites.google.com/view/ahutracking001/)| 234 Video pairs, the extension of RGBT210 |
| VOT-RGBT19| VOT Community：2019 |[VOT-RGBT2019](https://pan.baidu.com/s/1kYnTTWF9LIkrCH4NNsSlFQ) *CODE:TZYD* | 60 Video pairs, about 2W frame pairs, a sub-set of RGBT 234|
| VOT-RGBT20|VOT Community： 2020 | [VOT-RGBT2020](https://pan.baidu.com/s/1fNgAVk4siqP2p-b1M2ZGmg ) *CODE:TZYD*| 60 Video pairs, its data is the same with VOT-RGBT2019, but with different evaluation mechanism|
| LasHeR| TIP'2021 | [LasHeR](https://github.com/BUGPLEASEOUT/LasHeR) | train/test split, imaged in the head-up view, above 70W image pairs in total; 245 videos in the test set|
| VTUAV| CVPR'2022 |[VTUAV](https://zhang-pengyu.github.io/DUT-VTUAV/) | imaged in the top-down view by uav, long-term;176 videos in the test-st, which has around 3300 frames in average|
| MV-RGBT| Arxiv'2024 |[MV-RGBT](https://github.com/Zhangyong-Tang/MVRGBT) |122 video pairs. The data in this benchmark mainly focus on the modality validity.|

***Generated Data***
| Dataset | Publish  | GitHub| Introduction|
|--|--|--| --|
| LSS-Dataset(from RGB) | TCSVT'2021 | [LSS-Dataset](https://pan.baidu.com/s/1x2hiqb2lSo54_4CI_L9YeQhttps://pan.baidu.com/s/1x2hiqb2lSo54_4CI_L9YeQ) ,code(Ye5Q)| Generated from VID|
| LSS-Dataset(from TIR) | TCSVT'2021 | [LSS-Dataset](https://pan.baidu.com/s/1xD3Ox-9VbZnyRQSWOxQRNw),code(IHws) | Generated from TIR|

## Results
<table width="100%" height="100%">
    <tr> 
        <th colspan="1"></th> 
	<th colspan="1"></th> 
	<th colspan="1"></th> 
        <th colspan="2">GTOT</th> 
        <th colspan="2">RGBT210</th> 
        <th colspan="2">RGBT234</th> 
        <th colspan="3">LasHeR</th> 
    </tr>
    <tr>
    	<td> Methods</td>
    	<td>Venue</td>
	<td>Speed</td>
    	<td> PR</td>
    	<td> SR</td>
    	<td> PR</td>
    	<td> SR</td>
       	<td> PR</td>
    	<td> SR</td>
    	<td> PR</td>
    	<td> NPR</td>
    	<td> SR</td>
    </tr>
	<tr> 
    	<td>SiamSCR</td>
    	<td>IEEE Sensor Journal'2024</td>
	<td>37.2</td>
    	<td>91.7</td>
    	<td>73.7</td>
    	<td></td>
    	<td></td>
    	<td>79.1</td>
    	<td>57.5</td>
	<td>52.2</td>
       	<td></td>
    	<td>40.1</td>
    </tr>
	<tr> 
    	<td>SiamMGT</td>
    	<td>The Journal of Supercomputing'2024</td>
	<td></td>
    	<td>90.9</td>
    	<td>73.9</td>
    	<td></td>
    	<td></td>
    	<td>81.1</td>
    	<td>60.4</td>
	<td>54.8</td>
       	<td></td>
    	<td>41.6</td>
    </tr>
	<tr> 
    	<td>AINet</td>
    	<td>arxiv'2024</td>
	<td>37.5/4090</td>
    	<td></td>
    	<td></td>
    	<td>87.5</td>
    	<td>64.8</td>
    	<td>89.2</td>
    	<td>67.3</td>
	<td>74.2</td>
       	<td>70.1</td>
    	<td>59.1</td>
    </tr>
	<tr> 
    	<td>MambaVT</td>
    	<td>ARxiv'2024</td>
	<td>31.1/A100</td>
    	<td>95.2</td>
    	<td>78.6</td>
    	<td>88.5</td>
    	<td>64.4</td>
    	<td>90.7</td>
    	<td>67.5</td>
	<td>72.7</td>
       	<td>69.0</td>
    	<td>57.5</td>
    </tr>
	<tr> 
    	<td>AMAtrack</td>
    	<td>TIM'2024</td>
	<td>68.3/RTX3070</td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td>82.6</td>
    	<td>61.2</td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td>CAFormer</td>
    	<td>ARxiv'2024</td>
	<td>83.6/RTX3080Ti</td>
    	<td>91.8</td>
    	<td>76.9</td>
    	<td>85.6</td>
    	<td>63.2</td>
    	<td>88.3</td>
    	<td>66.4</td>
	<td>70.0</td>
       	<td>66.1</td>
    	<td>55.6</td>
    </tr>
<tr> 
    	<td>VLCTrack</td>
    	<td>NeuroComputing'2024</td>
	<td>90.9/RTX4090</td>
    	<td>90.1</td>
    	<td>76.8</td>
    	<td></td>
    	<td></td>
    	<td>81.1</td>
    	<td>59.1</td>
	<td>56.4</td>
       	<td>51.8</td>
    	<td>43.7</td>
    </tr>
<tr> 
    	<td>MixRGBX</td>
    	<td>NeuroComputing'2024</td>
	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td>85.3</td>
    	<td>63.2</td>
	<td>67.2</td>
       	<td></td>
    	<td>53.2</td>
    </tr>
<tr> 
    	<td>TGTrack</td>
    	<td>TCSVT'2024</td>
	<td></td>
    	<td></td>
    	<td></td>
    	<td>87.2</td>
    	<td>64.1</td>
    	<td>89.3</td>
    	<td>67.0</td>
	<td>73.2</td>
       	<td>69.1</td>
    	<td>57.9</td>
    </tr>
<tr> 
    	<td>CKD</td>
    	<td>ACMMM'2024</td>
	<td>96.4/4090 </td>
    	<td>92.5</td>
    	<td>75.1</td>
    	<td>88.4</td>
    	<td>65.2</td>
    	<td>90.0</td>
    	<td> 67.4</td>
	<td> 73.2</td>
       	<td> 69.4</td>
    	<td> 58.1</td>
    </tr>
<tr> 
    	<td>IIMF</td>
    	<td>ACMMM'2024</td>
	<td> </td>
    	<td></td>
    	<td> </td>
    	<td>85.6</td>
    	<td>62.4</td>
    	<td>86.8</td>
    	<td> 64.4</td>
	<td> 72.4</td>
       	<td> 68.4</td>
    	<td> 58.1</td>
    </tr>
<tr> 
    	<td>MMSTC</td>
    	<td>TIP'2024</td>
	<td> </td>
    	<td>94.1</td>
    	<td> 77.9</td>
    	<td>88.6</td>
    	<td>65.7</td>
    	<td>89.8</td>
    	<td> 67.3</td>
	<td> 72.3</td>
       	<td> 68.6</td>
    	<td> 57.4</td>
    </tr>
<tr> 
    	<td>MELT</td>
    	<td>ACMTOMM'2024</td>
	<td>20</td>
    	<td></td>
    	<td> </td>
    	<td></td>
    	<td></td>
    	<td>75.3</td>
    	<td> 54.6</td>
	<td> 57.3</td>
       	<td> 52.7</td>
    	<td> 45.0</td>
    </tr>
<tr> 
    	<td>TIH</td>
    	<td>PR'2024</td>
	<td> 72</td>
    	<td> 93.5</td>
    	<td> 77.0</td>
    	<td> </td>
    	<td> </td>
    	<td>89.4</td>
    	<td> 66.4</td>
	<td> 72.0</td>
       	<td> 67.7</td>
    	<td> 57.2</td>
    </tr>
<tr> 
    	<td>AMRT</td>
    	<td>electronics'2024</td>
	<td> 32.31</td>
    	<td>90.0</td>
    	<td> 73.0</td>
    	<td> </td>
    	<td> </td>
    	<td>84.4</td>
    	<td> 60.2</td>
	<td> 46.8</td>
       	<td> </td>
    	<td> 32.4</td>
    </tr>
<tr> 
    	<td>XTrack</td>
    	<td>Arxiv'2024</td>
	<td> -</td>
    	<td>-</td>
    	<td> -</td>
    	<td> </td>
    	<td> </td>
    	<td>84.8</td>
    	<td> 62.2</td>
	<td> 65.5</td>
       	<td> </td>
    	<td> 52.5</td>
    </tr>
<tr> 
    	<td>SeqTrackv2</td>
    	<td>Arxiv'2024</td>
	<td> -</td>
    	<td></td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    	<td>68.5</td>
    	<td> 92.3</td>
	<td> 76.7</td>
       	<td> </td>
    	<td> 61.0</td>
    </tr>
<tr> 
    	<td>KSTrack</td>
    	<td>TCSVT'2024</td>
	<td> -</td>
    	<td>95.5</td>
    	<td> 74.1</td>
    	<td> </td>
    	<td> </td>
    	<td>85.0</td>
    	<td> 58.7</td>
	<td> </td>
       	<td> </td>
    	<td> </td>
    </tr>
<tr> 
    	<td>MINet</td>
    	<td>IVC'2024</td>
	<td> -</td>
    	<td></td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    	<td>84.3</td>
    	<td> 62.9</td>
	<td> 65.9</td>
       	<td> </td>
    	<td> 52.9</td>
    </tr>
<tr> 
    	<td>BAT</td>
    	<td>AAAI'2024</td>
	<td> -</td>
    	<td>-</td>
    	<td> -</td>
    	<td> </td>
    	<td> </td>
    	<td> 86.8</td>
    	<td> 64.1</td>
	<td> 70.2</td>
       	<td> </td>
    	<td> 56.3</td>
    </tr>
	 <tr> 
    	<td>TATrack</td>
    	<td>AAAI'2024</td>
	<td> 26.1/RTX3090</td>
    	<td>-</td>
    	<td> -</td>
    	<td> 85.3</td>
    	<td> 61.8</td>
    	<td> 87.2</td>
    	<td> 64.4</td>
	<td> 70.2</td>
       	<td> 66.7</td>
    	<td> 56.1</td>
    </tr>
	 <tr> 
    	<td>GMMT</td>
    	<td>AAAI'2024</td>
	<td> 18/RTX3090Ti</td>
    	<td>93.6</td>
    	<td> 78.5</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 87.9</td>
    	<td> 64.7</td>
	<td> 70.7</td>
       	<td> 67.0</td>
    	<td> 56.6</td>
    </tr>
	 <tr> 
    	<td>LMINet</td>
    	<td>IEEE Sensors Journal'2024</td>
	<td> 5.6/V100</td>
    	<td>91.4</td>
    	<td> 73.6</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 83.8</td>
    	<td> 59.2</td>
	<td> 49.0</td>
       	<td> 43.3</td>
    	<td> 34.8</td>
    </tr>
	 <tr> 
    	<td> CAT++</td>
    	<td>TIP'2024</td>
	<td> 14/2080Ti</td>
    	<td>91.5</td>
    	<td> 73.3</td>
    	<td> 82.2</td>
    	<td> 56.1</td>
    	<td> 84.0</td>
    	<td> 59.2</td>
	<td> 50.9</td>
       	<td> 44.4</td>
    	<td> 34.8</td>
    </tr>
	 <tr> 
    	<td>AMNet</td>
    	<td>TCSVT'2024</td>
	<td> 14/2080Ti</td>
    	<td>92.9</td>
    	<td> 77.4</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 87.7</td>
    	<td> 65.5</td>
	<td> 70.2</td>
       	<td> 66.0</td>
    	<td> 55.9</td>
    </tr>
	 <tr> 
    	<td>MPLKD</td>
    	<td>Arxiv'2024</td>
	<td> 81.8/RTX3090</td>
    	<td>92.4</td>
    	<td> 77.3</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 87.3</td>
    	<td> 65.1</td>
	<td> 71.4</td>
       	<td> -</td>
    	<td> 56.7</td>
    </tr>
	 <tr> 
    	<td>QueryTrack<</td>
    	<td>TIP'2024</td>
	<td> 27/RTX A6000</td>
    	<td>92.3</td>
    	<td> 75.9</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 84.1</td>
    	<td> 60.0</td>
	<td> 66.0</td>
       	<td> -</td>
    	<td> 52.0</td>
	 </tr>
	 <tr> 
    	<td>MCTrack</td>
    	<td>TCSVT'2024</td>
	<td> -</td>
    	<td>94.1</td>
    	<td> 77.6</td>
    	<td> 86.4</td>
    	<td> 63.7</td>
    	<td> 87.5</td>
    	<td> 65.6</td>
	<td> 71.6</td>
       	<td> 67.6</td>
    	<td> 57.1</td>
    </tr>
	 <tr> 
    	<td> SDSTrack</td>
    	<td>CVPR'2024</td>
	<td> 21/RTX3090Ti</td>
    	<td>-</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 84.8</td>
    	<td> 62.5</td>
	<td> -</td>
       	<td> 66.5</td>
    	<td> 53.1</td>
    </tr>
	 <tr> 
    	<td>OneTracker</td>
    	<td>CVPR'2024</td>
	<td> -</td>
    	<td>-</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 85.7</td>
    	<td> 64.2</td>
	<td> -</td>
       	<td> 67.2</td>
    	<td> 53.8</td>
    </tr>
	 <tr> 
    	<td> UnTrack</td>
    	<td>CVPR'2024</td>
	<td> -</td>
    	<td>-</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 84.2</td>
    	<td> 62.5</td>
	<td> 66.7</td>
       	<td> -</td>
    	<td> 53.6</td>
    </tr>
<tr> 
    	<td> UStrack</td>
    	<td> IJCAI'2024</td>
	<td>84.2</td>
    	<td>93.4</td>
    	<td>78.3</td>
    	<td></td>
    	<td></td>
    	<td>87.4</td>
    	<td>65.8</td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
	 <tr> 
    	<td> AFter</td>
    	<td>Arxiv'2024</td>
	<td>23/RTX 4090</td>
    	<td>91.6</td>
    	<td> 78.5</td>
    	<td> 87.6</td>
    	<td> 63.5</td>
    	<td> 90.1</td>
    	<td> 66.7</td>
	<td> 70.3</td>
       	<td> 65.8</td>
    	<td> 55.1</td>
    </tr>
	 <tr> 
    	<td>CSTNet</td>
    	<td>Arxiv'2024</td>
	<td>-</td>
    	<td>-</td>
    	<td> -</td>
    	<td> 86.0</td>
    	<td> 63.5</td>
    	<td> 88.4</td>
    	<td> 65.2</td>
	<td> 71.5</td>
       	<td> 67.9</td>
    	<td> 57.2</td>
    </tr>
	 <tr> 
    	<td> CAFF</td>
    	<td>JSEE'2024</td>
	<td>-</td>
    	<td>85.2</td>
    	<td> 72.6</td>
    	<td> 71.5</td>
    	<td> 49.2</td>
    	<td> 74.0</td>
    	<td> 50.6</td>
	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td> SAFT</td>
    	<td>2024</td>
	<td>-</td>
    	<td>91.7</td>
    	<td> 73.9</td>
    	<td> -</td>
    	<td> *</td>
    	<td> 84.1</td>
    	<td> 57.3</td>
	<td> 51.1</td>
       	<td> -</td>
    	<td> 35.9</td>
    </tr>
 <tr> 
    	<td> IPL</td>
    	<td>Arxiv'2024</td>
	<td>-</td>
    	<td>91.7</td>
    	<td> 73.9</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 88.3</td>
    	<td> 65.7</td>
	<td> 69.4</td>
       	<td> 65.6</td>
    	<td> 55.3</td>
    </tr>
 <tr> 		
    	<td> MPT</td>
    	<td>TCSVT'2024</td>
	<td>-</td>
    	<td>-</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 76.9</td>
    	<td> 55.0</td>
	<td> 35.5</td>
       	<td> -</td>
    	<td> 31.3</td>
    </tr>
 <tr> 		
    	<td> MIGTD</td>
    	<td>PR'2024</td>
	<td>-</td>
    	<td>-</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 87.6</td>
    	<td> 65.8</td>
	<td> 72.0</td>
       	<td> 68.1</td>
    	<td> 57.2</td>
    </tr>
 <tr> 		
    	<td> Proformer</td>
    	<td>TCSVT'2024</td>
	<td>22</td>
    	<td>-</td>
    	<td> -</td>
    	<td> 86.8</td>
    	<td> 62.2</td>
    	<td> 89.9</td>
    	<td> 65.7</td>
	<td> 67.4</td>
       	<td> 63.0</td>
    	<td> 53.3</td>
    </tr>
 <tr> 		
    	<td> AWCM</td>
    	<td>TOMM'2024</td>
	<td>5/1080Ti</td>
    	<td>89.6</td>
    	<td>73.8</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 79.6</td>
    	<td> 56.9</td>
	<td> </td>
       	<td> </td>
    	<td> </td>
    </tr>
<tr> 
    	<td> FDAFT</td>
    	<td>PRCV'2023</td>
	<td> </td>
    	<td></td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    	<td> 88.2</td>
    	<td> 66.4</td>
    	<td> 68.9</td>
    	<td> -</td>
    	<td> 55.3</td>
    </tr>
<tr> 
    	<td> DFAT</td>
    	<td>INFFUS'2023</td>
	<td> 22/RTX2080Ti</td>
    	<td>0.893</td>
    	<td> 0.723</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.758</td>
    	<td> 0.552</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.336</td>
    </tr>
       <tr> 
    	<td> ViPT</td>
    	<td>CVPR'2023</td>
	<td> -</td>
    	<td>-</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.835</td>
    	<td> 0.617</td>
    	<td> 0.651</td>
    	<td> -</td>
    	<td> 0.525</td>
    </tr>
       <tr> 
    	<td>CMD</td>
    	<td>CVPR'2023</td>
	<td> 30/RTX1080Ti</td>
    	<td>0.892</td>
    	<td> 0.734</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.824</td>
    	<td> 0.584</td>
    	<td> 0.590</td>
    	<td> 0.546</td>
    	<td> 0.464</td>
    </tr>
       <tr> 
    	<td> TBSI</td>
    	<td>CVPR'2023</td>
	<td> 36/RTX3080Ti</td>
    	<td>-</td>
    	<td> -</td>
    	<td> 0.853</td>
    	<td> 0.625</td>
    	<td> 0.871</td>
    	<td> 0.637</td>
    	<td> 0.692</td>
    	<td> 0.657</td>
    	<td> 0.556</td>
    </tr>
       <tr> 
    	<td>BD2Track</td>
    	<td>SPL'2023</td>
	<td> -</td>
    	<td>-</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.560</td>
    	<td> -</td>
    	<td> 0.432</td>
    </tr>
       <tr> 
    	<td> SiamTDR</td>
    	<td>TICPS'2023</td>
	<td> 127/RTX3090</td>
    	<td>88.5</td>
    	<td> 71.4</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
       <tr> 
    	<td>SiamAFTS</td>
    	<td>ScienticReport'2023</td>
	<td> -</td>
    	<td>84.9</td>
    	<td> 77.7</td>
    	<td> 87.3</td>
    	<td> 56.4</td>
    	<td> 89.0</td>
    	<td> 60.2</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td>UMT</td>
    	<td>AIEA'2023</td>
	<td> 3/GTX1080Ti</td>
    	<td>89.2</td>
    	<td> 73.0</td>
    	<td> </td>
    	<td> </td>
    	<td> 84.2</td>
    	<td> 60.3</td>
	<td> 49.3</td>
       	<td> 43.0</td>
    	<td> 36.9</td>
    </tr>
	 <tr> 
    	<td>MPDMT</td>
    	<td>ICPR'2023</td>
	<td> 40/RTX3080</td>
    	<td>90.6</td>
    	<td> 75.7</td>
    	<td> </td>
    	<td> </td>
    	<td> 80.6</td>
    	<td> 58.3</td>
	<td> </td>
       	<td> </td>
    	<td> </td>
    </tr>	
<tr> 
    	<td> RSFNet</td>
    	<td>SPL'2023</td>
	<td> 83/RTX3090</td>
    	<td>92.1</td>
    	<td> 75.3</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 86.3</td>
    	<td> 62.2</td>
	<td> 65.9</td>
       	<td> -</td>
    	<td> 52.6</td>
    </tr>
<tr> 
    	<td> QAT</td>
    	<td>ACMMM'2023</td>
	<td> 22/</td>
    	<td>91.5</td>
    	<td> 75.5</td>
    	<td> 86.8</td>
    	<td> 61.9</td>
    	<td> 88.4</td>
    	<td> 64.3</td>
	<td> 64.2</td>
       	<td> 59.6</td>
    	<td> 50.1</td>
    </tr>
<tr> 
    	<td> PRO</td>
    	<td>CCDC'2023</td>
	<td></td>
    	<td>-</td>
    	<td> -</td>
    	<td> 68.0</td>
    	<td> 47.8</td>
    	<td> -</td>
    	<td> -</td>
	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    </tr>
<tr> 
    	<td> DFNet</td>
    	<td>TIST'2023</td>
	<td></td>
    	<td>88.1</td>
    	<td> 71.9</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 77.2</td>
    	<td> 51.3</td>
	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    </tr>
<tr> 
    	<td> DTAN</td>
    	<td>Cognitive Computation'2023</td>
	<td>0.5</td>
    	<td>88.</td>
    	<td> 71.5</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 78.2</td>
    	<td> 55.1</td>
	<td> 57.5</td>
       	<td> 51.6</td>
    	<td> 41.0</td>
    </tr>
<tr> 
    	<td> DECFNet</td>
    	<td>ICMA'2023</td>
	<td>27.6</td>
    	<td>90.4</td>
    	<td> 70.8</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
	<td> 49.6</td>
       	<td> -</td>
    	<td> 35.0</td>
    </tr>
<tr> 
    	<td> DMSTM</td>
    	<td>TIM'2023</td>
	<td></td>
    	<td>92.9</td>
    	<td> 75.9</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 78.6</td>
    	<td> 56.2</td>
	<td> 54.1</td>
       	<td> 49.4</td>
    	<td> 40.0</td>
    </tr>
<tr> 
    	<td> SiamFEA</td>
    	<td>JVCIR'2023</td>
	<td></td>
    	<td>92.0</td>
    	<td> 76.6</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 83.7</td>
    	<td> 61.7</td>
	<td> 64.5</td>
       	<td> -</td>
    	<td> 50.9</td>
    </tr>
<tr> 
    	<td> HATFNet</td>
    	<td>Applied Intelligence'2023</td>
	<td>9.8</td>
    	<td>91.8/td>
    	<td> 77.3</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 80.7</td>
    	<td> 59.5</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> MACFT</td>
    	<td>Sensors'2023</td>
	<td>31</td>
    	<td>-/td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 85.7</td>
    	<td> 62.2</td>
	<td>65.3</td>
       	<td> -</td>
    	<td>51.4</td>
    </tr>
<tr> 
    	<td> LCMIT</td>
    	<td>SCIENCE CHINA Information Sciences'2023</td>
	<td></td>
    	<td>93.9/td>
    	<td> 74.1</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 83.1</td>
    	<td> 57.8</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> MMMPT</td>
    	<td>IPT'2023</td>
	<td></td>
    	<td>90.3/td>
    	<td> 73.6</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 79.8</td>
    	<td> 54.6</td>
	<td>53.0</td>
       	<td> -</td>
    	<td>40.0</td>
    </tr>
<tr> 
    	<td> MPDMT</td>
    	<td>ICPR'2023</td>
	<td>42</td>
    	<td>90.6/td>
    	<td> 75.7</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 80.7</td>
    	<td> 58.3</td>
	<td>53.0</td>
       	<td> -</td>
    	<td>40.0</td>
    </tr>
<tr> 
    	<td> FSBNet</td>
    	<td>Neural Computing and Applications'2023</td>
	<td>27</td>
    	<td>91.3/td>
    	<td> 72.1</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 82.4</td>
    	<td> 56.2</td>
	<td>53.7</td>
       	<td> -</td>
    	<td>42.5</td>
    </tr>
<tr> 
    	<td> MTNet</td>
    	<td>ICME'2023</td>
	<td>-</td>
    	<td>93.5/td>
    	<td>76.0</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 85.0</td>
    	<td> 61.9</td>
	<td>60.8</td>
       	<td> -</td>
    	<td>47.4</td>
    </tr>
<tr> 
    	<td> SiamMFF</td>
    	<td>CACML'2023</td>
	<td>-</td>
    	<td>90.5/td>
    	<td>73.6</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 81.2</td>
    	<td> 57.3</td>
	<td>60.8</td>
       	<td> -</td>
    	<td>47.4</td>
    </tr>
<tr> 
    	<td> LSAR</td>
    	<td>TCSVT'2023</td>
	<td>-</td>
    	<td>85.5/td>
    	<td>70.3</td>
    	<td>77.5</td>
    	<td>54.9</td>
    	<td> 78.4</td>
    	<td> 55.9</td>
	<td>46.0</td>
       	<td> -</td>
    	<td>38.5</td>
    </tr>
<tr> 
    	<td> CSMMA</td>
    	<td>Sensors Journal'2023</td>
	<td>20</td>
    	<td>89.5/td>
    	<td>73.0</td>
    	<td>-</td>
    	<td>-</td>
    	<td> 77.8</td>
    	<td> 53.2</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> MPLT</td>
    	<td>Arxiv'2023</td>
	<td></td>
    	<td>-/td>
    	<td>-</td>
    	<td>86.2</td>
    	<td>63.0</td>
    	<td>88.4</td>
    	<td>65.7</td>
	<td>72.0</td>
       	<td> -</td>
    	<td>57.1</td>
    </tr>
<tr> 
    	<td> CRSP</td>
    	<td>ICIP'2023</td>
	<td>-</td>
    	<td>90.4</td>
    	<td>77.2</td>
    	<td>74.0</td>
    	<td>63.2</td>
    	<td>-</td>
    	<td>-</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> GABBP</td>
    	<td>TNNLS'2023</td>
	<td>-</td>
    	<td>90.3</td>
    	<td>77.2</td>
    	<td>68.6</td>
    	<td>68.5</td>
    	<td>-</td>
    	<td>59.7</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> PLASSO-ADSPF</td>
    	<td>KBS'2023</td>
	<td>63</td>
    	<td>-</td>
    	<td>-</td>
    	<td>-</td>
    	<td>-</td>
    	<td>82.7</td>
    	<td>59.2</td>
	<td>54.7</td>
       	<td> -</td>
    	<td>47.4</td>
    </tr>
<tr> 
    	<td> SRCDCF</td>
    	<td>IPT'2023</td>
	<td>53</td>
    	<td>83.0</td>
    	<td>65.3</td>
    	<td>66.3</td>
    	<td>47.5</td>
    	<td>66.9</td>
    	<td>47.8</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> MFENet</td>
    	<td>Multimedia Tools and Applications'2023</td>
	<td>1.43</td>
    	<td>89.8</td>
    	<td>71.9</td>
    	<td>-</td>
    	<td>-</td>
    	<td>83.2</td>
    	<td>57.1</td>
	<td>51.7</td>
       	<td> -</td>
    	<td>37.4</td>
    </tr>
<tr> 
    	<td> RMFNet</td>
    	<td> Applied Sciences'2023</td>
	<td>10</td>
    	<td>91.1</td>
    	<td>76.9</td>
    	<td>-</td>
    	<td>-</td>
    	<td>79.4</td>
    	<td>58.5</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> M2GCI</td>
    	<td> NPL'2023</td>
	<td></td>
    	<td>90.9</td>
    	<td>73.7</td>
    	<td>-</td>
    	<td>-</td>
    	<td>79.3</td>
    	<td>56.9</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> SiamIVFN</td>
    	<td> JMLC'2023</td>
	<td>147</td>
    	<td>91.5</td>
    	<td>79.3</td>
    	<td>-</td>
    	<td>-</td>
    	<td>81.1</td>
    	<td>63.2</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> STRT</td>
    	<td> Applied Intelligence'2023</td>
	<td>15</td>
    	<td>91.3</td>
    	<td>74.4</td>
    	<td>80.2</td>
    	<td>56.8</td>
    	<td>83.6</td>
    	<td>60.4</td>
	<td>63.6</td>
       	<td>59.4</td>
    	<td>50.0</td>
    </tr>
<tr> 
    	<td> SGF_MDNet+RGBT</td>
    	<td> IET Image Processinge'2023</td>
	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td>73.8</td>
    	<td>56.3</td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td> SiamCAF</td>
    	<td> Remote Sensing'2023</td>
	<td></td>
    	<td>90.6</td>
    	<td>73.0</td>
    	<td></td>
    	<td></td>
    	<td>77.1</td>
    	<td>53.7</td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td> TEFNet</td>
    	<td> PRCV'2023</td>
	<td>25.5</td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
	<td>63.1</td>
       	<td>59.1</td>
    	<td>50.1</td>
    </tr>
<tr> 
    	<td> DAPF</td>
    	<td> Multimedia Tools and Applications'2023</td>
	<td>1.16</td>
    	<td>-</td>
    	<td></td>
    	<td>-</td>
    	<td></td>
    	<td>86.0</td>
    	<td>62.0</td>
	<td>71.1</td>
       	<td></td>
    	<td>51.6</td>
    </tr>
<tr> 
    	<td> UDT-FF</td>
    	<td> Multimedia Tools and Applications'2023</td>
	<td>71.9</td>
    	<td>79.3</td>
    	<td>65.1</td>
    	<td>-</td>
    	<td></td>
    	<td>56.1</td>
    	<td>41.4</td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td> UMT</td>
    	<td> AIEA'2023</td>
	<td></td>
    	<td>89.2</td>
    	<td>73.0</td>
    	<td>-</td>
    	<td></td>
    	<td>84.2</td>
    	<td>60.3</td>
	<td>49.3</td>
       	<td>43.0</td>
    	<td>36.9</td>
    </tr>
<tr> 
    	<td> CSRDCF_RGBT</td>
    	<td> IEEE SENSORS JOURNAL'2023</td>
	<td></td>
    	<td></td>
    	<td></td>
    	<td>-</td>
    	<td></td>
    	<td>70.7</td>
    	<td>51.4</td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td> APFNet</td>
    	<td>AAAI'2022</td>
	<td> -</td>
    	<td>0.905</td>
    	<td> 0.739</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.827</td>
    	<td> 0.579</td>
    	<td> 0.500</td>
    	<td> -</td>
    	<td> 0.362</td>
    </tr>
    <tr> 
    	<td> TAAT</td>
    	<td>arxiv'2022</td>
	<td> 39/RTX2080Ti</td>
    	<td>0.858</td>
    	<td> 0.696</td>
    	<td> 0.710</td>
    	<td> 0.486</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
 	<tr> 
    	<td> DMCNet</td>
    	<td>TNNLS'2022</td>
	<td> 2.38/RTX2080Ti</td>
    	<td>0.909</td>
    	<td> 0.733</td>
    	<td> 0.797</td>
    	<td> 0.555</td>
    	<td> 0.839</td>
    	<td> 0.593</td>
    	<td> 0.490</td>
    	<td> 0.431</td>
    	<td> 0.355</td>
    </tr>
    </tr>
 	<tr> 
    	<td> MFGNet</td>
    	<td>TMM'2022</td>
	<td> 3.37/Tesla P100</td>
    	<td>0.889</td>
    	<td> 0.707</td>
    	<td> 0.749</td>
    	<td> 0.494</td>
    	<td> 0.783</td>
    	<td> 0.535</td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    </tr>
 	<tr> 
    	<td> HMFT</td>
    	<td>CVPR'2022</td>
	<td> 30/GTXTitan</td>
    	<td>0.912</td>
    	<td> 0.749</td>
    	<td> 0.786</td>
    	<td> 0.535</td>
    	<td> 0.788</td>
    	<td> 0.568</td>
    	<td> 0.460</td>
    	<td> 0.413</td>
    	<td> 0.326</td>
    </tr>
       <tr> 
    	<td> ProTrack </td>
    	<td>ACMMM'2022</td>
	<td> -</td>
    	<td>-</td>
    	<td> -</td>
    	<td> -</td>
    	<td> </td>
    	<td> 78.6</td>
    	<td> 58.7</td>
    	<td> 50.9</td>
    	<td> </td>
    	<td> 42.1</td>
    </tr>
<tr> 
    	<td> AGMINet</td>
    	<td>TIM'2022</td>
	<td>8.8</td>
    	<td>91.7</td>
    	<td> 73.4</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 84.0</td>
    	<td> 59.2</td>
    	<td> 48.8</td>
    	<td> 42.9</td>
    	<td> 34.3</td>
    </tr>
<tr> 
    	<td> CMC2R</td>
    	<td>IET Image Processing'2022</td>
	<td></td>
    	<td></td>
    	<td> </td>
    	<td> -</td>
    	<td> -</td>
    	<td> 73.2</td>
    	<td> 52.6</td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    </tr>
<tr> 
    	<td> DuSiamRT</td>
    	<td>The Visual Computer'2022</td>
	<td>116</td>
    	<td>76.6</td>
    	<td>62.8</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 56.7</td>
    	<td> 38.4</td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    </tr>
<tr> 
    	<td> SiamCSR</td>
    	<td>IGARSS'2022</td>
	<td>140</td>
    	<td>88.2</td>
    	<td>70.9</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 75.4</td>
    	<td> 53.2</td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    </tr>
<tr> 
    	<td> LRMWT</td>
    	<td>KBS'2022</td>
	<td>24.6</td>
    	<td>91.1</td>
    	<td>75.3</td>
    	<td>80.6</td>
    	<td>59.2</td>
    	<td> 82.5</td>
    	<td> 61.6</td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    </tr>
<tr> 
    	<td> MIRNet</td>
    	<td>ICME'2022</td>
	<td></td>
    	<td>90.9</td>
    	<td>74.4</td>
    	<td></td>
    	<td></td>
    	<td> 81.6</td>
    	<td> 58.9</td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    </tr>
<tr> 
    	<td> MBAFNet</td>
    	<td>IEEE Sensors Journal'2022</td>
	<td>15.2</td>
    	<td>91.6</td>
    	<td>76.7</td>
    	<td></td>
    	<td></td>
    	<td> 80.1</td>
    	<td> 58.5</td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    </tr>
<tr> 
    	<td> RSF</td>
    	<td>Science China Information Sciences'2022</td>
	<td></td>
    	<td>86.4</td>
    	<td>70.7</td>
    	<td></td>
    	<td></td>
    	<td> 66.6</td>
    	<td> 48.4</td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    </tr>
<tr> 
    	<td> CF-LG</td>
    	<td>IVC'2022</td>
	<td>32.29</td>
    	<td>94.7</td>
    	<td>65.5</td>
    	<td>71.5</td>
    	<td>49.0</td>
    	<td> 71.7</td>
    	<td> 49.3</td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    </tr>
<tr> 
    	<td> MFNet</td>
    	<td>IVC'2022</td>
	<td>19</td>
    	<td>90.7</td>
    	<td>73.5</td>
    	<td>71.5</td>
    	<td>49.0</td>
    	<td>84.4</td>
    	<td>60.1</td>
    	<td>59.7</td>
    	<td>55.4</td>
    	<td>46.7</td>
    </tr>
<tr> 
    	<td> RLTN</td>
    	<td>JEI'2022</td>
	<td>1.06</td>
    	<td>89.3</td>
    	<td>73.8</td>
    	<td></td>
    	<td></td>
    	<td>77.1</td>
    	<td>55.5</td>
    	<td></td>
    	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td> TFNet</td>
    	<td>TCSVT'2022</td>
	<td>20</td>
    	<td>88.6</td>
    	<td>72.9</td>
    	<td>77.7</td>
    	<td>52.9</td>
    	<td>80.6</td>
    	<td>56.0</td>
    	<td></td>
    	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td> SCA_MMA</td>
    	<td>ELECTRONICS'2022</td>
	<td>1.3</td>
    	<td>90.5</td>
    	<td>73.2</td>
    	<td></td>
    	<td></td>
    	<td>80.2</td>
    	<td>56.9</td>
    	<td></td>
    	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td> SiamMFF</td>
    	<td>Machine Vision and Applications'2022</td>
	<td></td>
    	<td>85.8</td>
    	<td>71.1</td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td> JMMAC</td>
    	<td>TIP'2021</td>
	<td> 4/RTX2080Ti</td>
    	<td>90.2</td>
    	<td> 73.2</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 79.0</td>
    	<td> 57.3</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>		
      	<tr> 
    	<td>MANet++</td>
    	<td>TIP'2021</td>
	<td> -</td>
    	<td>90.1</td>
    	<td> 72.3</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 80.0</td>
    	<td> 55.4</td>
    	<td> 46.7</td>
    	<td> 40.4</td>
    	<td> 31.4</td>
    </tr>
       	<tr> 
    	<td> CBPNet</td>
    	<td>TMM'2021</td>
	<td> -</td>
    	<td>88.5</td>
    	<td> 71.6</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 79.4</td>
    	<td> 54.1</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
       	<tr> 
    	<td> CEDiMP</td>
    	<td>Sensors'2021</td>
	<td> -</td>
    	<td>88.6</td>
    	<td> 73.1</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 80.8</td>
    	<td> 56.1</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
        <tr> 
    	<td>FANet</td>
    	<td>TIV'2021</td>
	<td> 19/RTX2080Ti</td>
    	<td>89.1</td>
    	<td> 72.8</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 78.7</td>
    	<td> 55.3</td>
    	<td> 44.1</td>
    	<td> 38.4</td>
    	<td> 30.9</td>
    </tr>
         <tr> 
    	<td> ADRNet</td>
    	<td>IJCV'2021</td>
	<td> 25/RTX2080Ti</td>
    	<td>90.4</td>
    	<td> 73.9</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 80.9</td>
    	<td> 57.1</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
	<tr> 
    	<td>M^5L</td>
    	<td>TIP'2021</td>
	<td> -</td>
    	<td>0.896</td>
    	<td> 0.710</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.795</td>
    	<td> 0.542</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
            <tr> 
    	<td> SiamCDA</td>
    	<td>TCSVT'2021</td>
		<td> -</td>
    	<td>0.877</td>
    	<td> 0.732</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.760</td>
    	<td> 0.569</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
   <tr> 
    	<td> EStaple</td>
    	<td>JCSC'2021</td>
	<td> 44/AMD3950</td>
    	<td>-</td>
    	<td> </td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.648</td>
    	<td> 0.470</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
   <tr> 
    	<td> AFCF</td>
    	<td>TITS'2021</td>
	<td> </td>
    	<td>93.1</td>
    	<td>64.0</td>
    	<td> 65.7</td>
    	<td> 46.9</td>
    	<td>66.4</td>
    	<td>47.2</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
   <tr> 
    	<td> HDINet</td>
    	<td>IEEE Sensors Journal'2021</td>
	<td> </td>
    	<td>88.8</td>
    	<td>71.8</td>
    	<td></td>
    	<td> </td>
    	<td>78.3</td>
    	<td>55.9</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
   <tr> 
    	<td> NRCMR</td>
    	<td>TNNLS'2021</td>
	<td>7.0</td>
    	<td>83.7</td>
    	<td>66.4</td>
    	<td></td>
    	<td> </td>
    	<td>72.9</td>
    	<td>50.2</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
   <tr> 
    	<td> CMMP</td>
    	<td>Neurocomputing'2021</td>
	<td>35.0</td>
    	<td>86.9</td>
    	<td>71.1</td>
    	<td></td>
    	<td> </td>
    	<td>75.1</td>
    	<td>49.1</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
	<tr> 
    	<td> MaCNet</td>
    	<td> Sensors'2020</td>
		<td> -</td>
    	<td>0.880</td>
    	<td> 0.714</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.790</td>
    	<td> 0.554</td>
    	<td> 0.482</td>
    	<td> 0.420</td>
    	<td> 0.350</td>
    </tr>
   	<tr> 
    	<td>CMPP</td>
    	<td>CVPR'2020</td>
	<td> 1.3/RTX2080Ti</td>
    	<td>0.926</td>
    	<td> 0.738</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.823</td>
    	<td> 0.575</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    	<tr> 
    	<td>CAT</td>
    	<td>ECCV'2020</td>
	<td> -</td>
    	<td>0.889</td>
    	<td> 0.717</td>
    	<td> 0.792</td>
    	<td> 0.533</td>
    	<td> 0.804</td>
    	<td> 0.561</td>
    	<td> 0.450</td>
    	<td> 0.395</td>
    	<td> 0.314</td>
    </tr>
    	<tr> 
    	<td> DSiamMFT</td>
    	<td>2020</td>
	<td> 14.7/RTX1080Ti</td>
    	<td>-</td>
    	<td> -</td>
    	<td> 0.642</td>
    	<td> 0.432</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    	<tr> 
    	<td> LDUA-STRCF</td>
    	<td>JVCIR'2020</td>
	<td>12.65</td>
    	<td>-</td>
    	<td> -</td>
    	<td>76.0</td>
    	<td>54.6</td>
    	<td> 78.3</td>
    	<td> 58.1</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    	<tr> 
    	<td> MECF</td>
    	<td>ICMCCE'2020</td>
	<td>11</td>
    	<td>-</td>
    	<td> -</td>
    	<td>69.0</td>
    	<td>50.2</td>
    	<td> </td>
    	<td> </td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
	<tr> 
    	<td> mfDiMP</td>
    	<td> ICCVW'2019</td>
	<td> 28/GTXTitan</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.786</td>
    	<td> 0.555</td>
    	<td> 0.785</td>
    	<td> 0.559</td>
    	<td> 0.448</td>
    	<td> 0.395</td>
    	<td> 0.343</td>
    </tr>
    <tr> 
    	<td> MANet </td>
    	<td> ICCVW'2019</td>
	<td> -</td>
    	<td> 0.894</td>
    	<td> 0.724</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.777</td>
    	<td> 0.539</td>
    	<td> 0.457</td>
    	<td> -</td>
    	<td> 0.330</td>
    </tr>
      <tr> 
    	<td>DAPNet</td>
    	<td> ACM MM'2019</td>
	<td> -</td>
    	<td> 0.882</td>
    	<td> 0.707</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.766</td>
    	<td> 0.537</td>
    	<td> 0.431</td>
    	<td> -</td>
    	<td> 0.314</td>
    </tr>
       <tr> 
    	<td> DAFNet</td>
    	<td> ICCVW'2019</td>
	<td> -</td>
    	<td> 0.891</td>
    	<td> 0.712</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.796</td>
    	<td> 0.544</td>
    	<td> 0.448</td>
    	<td> 0.390</td>
    	<td> 0.311</td>
    </tr>
            <tr> 
    	<td>SiamFT</td>
    	<td> IEEE Access'2019</td>
	<td> 30/RTX1080Ti</td>
    	<td>0.826</td>
    	<td> 0.700</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.688</td>
    	<td> 0.486</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
            <tr> 
    	<td>CMCFT</td>
    	<td> Neurocomputing'2019</td>
	<td> </td>
    	<td>77.0</td>
    	<td> 63.2</td>
    	<td> 52.9</td>
    	<td> 36.6</td>
    	<td> </td>
    	<td></td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
            <tr> 
    	<td>LGMG</td>
    	<td> TCSVT'2019</td>
	<td>7 </td>
    	<td>82.9</td>
    	<td> 65.5</td>
    	<td> 71.1</td>
    	<td> 46.8</td>
    	<td> 0.688</td>
    	<td> 0.486</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
        <tr> 
    	<td>LTODA</td>
    	<td> Arxiv'2019</td>
	<td></td>
    	<td>84.3</td>
    	<td> 67.7</td>
    	<td> </td>
    	<td> </td>
    	<td> 76.7</td>
    	<td>54.5</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td>fusionnet<td>
    	<td> NeuroComputing'2018</td>
	<td> -</td>
    	<td> 85.2</td>
    	<td> 62.6</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td>CMR<td>
    	<td> ECCV'2018</td>
	<td> -</td>
    	<td> 82.7</td>
    	<td> 64.3</td>
    	<td> 69.4</td>
    	<td> 46.3</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td>SCCF<td>
    	<td> PRCV'2018</td>
	<td> -</td>
    	<td> 85.0</td>
    	<td> 68.1</td>
    	<td> </td>
    	<td> </td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td>LMDCN<td>
    	<td> CISP'2018</td>
	<td> -</td>
    	<td></td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    	<td>61.7</td>
    	<td>38.7</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td>TMGRMR<td>
    	<td> Signal Processing: Image Communication'2018</td>
	<td>7</td>
    	<td>84.2</td>
    	<td>62.2</td>
    	<td> </td>
    	<td> </td>
    	<td></td>
    	<td></td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
</table>

### VTUAV/VOT-RGBT2019/2020

<table>
    <tr> 
        <th colspan="1"></th> 
        <th colspan="1"></th> 
	<th colspan="1"></th> 
        <th colspan="3">VTUAV</th> 
        <th colspan="3">VOT-RGBT2019</th> 
        <th colspan="3">VOT-RGBT2020</th> 
    </tr>
    <tr>
    	<td> Methods</td>
    	<td>Venue</td>
	<td>Speed</td>
    	<td> PR</td>
    	<td> NPR</td>
    	<td> SR</td>
       	<td> R</td>
    	<td> A</td>
    	<td> EAO</td>
    	<td> R</td>
    	<td> A</td>
    	<td> EAO</td> 	
    </tr>
	<tr> 
    	<td>AINet</td>
    	<td>arxiv'2024</td>
	<td>37.5/4090</td>
	<td> 88.0</td>
    	<td> </td>
    	<td> 75.3</td>
       	<td> </td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    	<td> </td>
    	<td> </td> 	
    </tr>
<tr> 
    	<td>CAFormer</td>
    	<td>Arxiv'2024</td>
	<td>83.6/RTX3080Ti</td>
    	<td>88.6</td>
    	<td> </td>
    	<td>76.2</td>
    	<td></td>
    	<td></td>
    	<td></td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td>CKD</td>
    	<td>ACMMM'2024</td>
	<td>96.4/4090</td>
    	<td>90.2</td>
    	<td> </td>
    	<td>77.8</td>
    	<td></td>
    	<td></td>
    	<td></td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td>MMSTC</td>
    	<td>TIP'2024</td>
	<td> </td>
    	<td>83.9</td>
    	<td> </td>
    	<td>67.7</td>
    	<td></td>
    	<td></td>
    	<td></td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td>MELT</td>
    	<td>ACMTOMM'2024</td>
	<td>20</td>
    	<td>68.3</td>
    	<td> </td>
    	<td>55.6</td>
    	<td>83.2</td>
    	<td>65.2</td>
    	<td>50.8</td>
	<td> </td>
       	<td> </td>
    	<td> </td>
    </tr>
 <tr> 		
    	<td> MIGTD</td>
    	<td>PR'2024</td>
	<td>26.9</td>
    	<td>88.3</td>
    	<td> -</td>
    	<td> 75.5</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    </tr>
 <tr> 		
    	<td> Proformer</td>
    	<td>TCSVT'2024</td>
	<td>22</td>
    	<td>84.6</td>
    	<td> -</td>
    	<td> 71.0</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    </tr>
 <tr> 
    	<td> IPL</td>
    	<td>Arxiv'2024</td>
	<td>-</td>
    	<td>87.5</td>
    	<td> -</td>
    	<td> 75.6</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    </tr>
 <tr> 		
    	<td> MPT</td>
    	<td>TCSVT'2024</td>
	<td>-</td>
    	<td>66.1</td>
    	<td> -</td>
    	<td> 54.1</td>
    	<td> 57.2</td>
    	<td> 79.1</td>
    	<td> 35.6</td>
	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td>MPLKD</td>
    	<td>Arxiv'2024</td>
	<td> 81.8/RTX3090</td>
    	<td>80.2</td>
    	<td> -</td>
    	<td> 67.4</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	 <tr> 
    	<td>QueryTrack</td>
    	<td>TIP'2024</td>
	<td> 27/RTX A6000</td>
    	<td> 75.5</td>
    	<td> -</td>
    	<td> 63.3</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
	 </tr>
<tr> 
    	<td> UStrack</td>
    	<td> IJCAI'2024</td>
	<td>84.2</td>
    	<td>86.9</td>
    	<td></td>
    	<td>74.4</td>
    	<td></td>
    	<td></td>
    	<td></td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
	 <tr> 
    	<td> AFter</td>
    	<td>Arxiv'2024</td>
	<td>RTX 4090/23</td>
    	<td> 84.9</td>
    	<td> -</td>
    	<td> 72.5</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td>CAFF</td>
    	<td>JSEE'2024</td>
	<td>-</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> 56.9</td>
    	<td> 52.9</td>
    	<td> 30.0</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
<tr> 
    	<td> DBDFAN</td>
    	<td>Drones'2023</td>
	<td>31.2</td>
    	<td>64.2</td>
    	<td>-</td>
    	<td> 51.6</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    </tr>
       <tr> 
    	<td> DFAT</td>
    	<td>INFFUS'2023</td>
	<td> 22/RTX2080Ti</td>
        <td> -</td>
    	<td> -</td>
    	 <td> -</td>
    	<td> 0.670</td>
       	<td> 0.756</td>
    	<td> 0.413</td>
    	<td>0.672</td>
        <td> 0.779</td>
    	<td> 0.390</td>
    </tr>
<tr> 
    	<td> DTAT</td>
    	<td>JIPS'2023</td>
	<td></td>
    	<td>61.3</td>
    	<td> -</td>
    	<td> 51.2.</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    </tr>
<tr> 
    	<td> MACFT</td>
    	<td>Sensors'2023</td>
	<td>31</td>
    	<td>80.1/td>
    	<td> -</td>
    	<td> 66.8</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> LSAR</td>
    	<td>TCSVT'2023</td>
	<td>8</td>
    	<td>42.7/td>
    	<td>-</td>
    	<td> 36.3</td>
    	<td>81.1</td>
    	<td>61.6</td>
    	<td> 40.0</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> CSMMA</td>
    	<td>Sensors Journal'2023</td>
	<td>20</td>
    	<td>-</td>
    	<td>-</td>
    	<td>-</td>
    	<td>66.1</td>
    	<td>60.5</td>
    	<td>38.7</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
	 <tr> 
    	<td>STRT</td>
    	<td>Applied Intelligence'2023</td>
	<td> 15/GTX1080Ti</td>
    	<td> 69.2</td>
    	<td> -</td>
    	<td> 57.2</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
<tr> 
    	<td> LCMIT</td>
    	<td>SCIENCE CHINA Information Sciences'2023</td>
	<td></td>
    	<td>-/td>
    	<td>-</td>
    	<td> -</td>
    	<td> 71.6</td>
    	<td> 62.5</td>
    	<td>38.1</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> MMMPT</td>
    	<td>IPT'2023</td>
	<td></td>
    	<td>73.1/td>
    	<td> -</td>
    	<td> 60.2</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
	<td>-</td>
       	<td> -</td>
    	<td>-</td>
    </tr>
<tr> 
    	<td> PLASSO-ADSPF</td>
    	<td>KBS'2023</td>
	<td>63</td>
    	<td>-</td>
    	<td>-</td>
    	<td>-</td>
    	<td>-</td>
    	<td>-</td>
    	<td>-</td>
	<td>81.2</td>
       	<td>67.0</td>
    	<td>49.9</td>
    </tr>
<tr> 
    	<td> SRCDCF</td>
    	<td>IPT'2023</td>
	<td>53</td>
    	<td>-</td>
    	<td>-</td>
    	<td>-</td>
    	<td>-</td>
    	<td>-</td>
    	<td>-</td>
	<td>72.0</td>
       	<td>61.7</td>
    	<td>37.0</td>
    </tr>
<tr> 
    	<td> SiamCAF</td>
    	<td> Remote Sensing'2023</td>
	<td></td>
    	<td>67.0</td>
    	<td></td>
    	<td>54.1</td>
    	<td></td>
    	<td></td>
    	<td></td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td> QAT</td>
    	<td>ACMMM'2023</td>
	<td> 22/</td>
    	<td> 80.1</td>
    	<td> -</td>
    	<td> 66.7</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
<tr> 
    	<td> TEFNet</td>
    	<td> PRCV'2023</td>
	<td>25.5</td>
    	<td>75.8</td>
    	<td></td>
    	<td>64.9</td>
    	<td></td>
    	<td></td>
    	<td></td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
<tr> 
    	<td> CSRDCF_RGBT</td>
    	<td> IEEE SENSORS JOURNAL'2023</td>
	<td></td>
    	<td>65.3</td>
    	<td></td>
    	<td>56.1</td>
    	<td></td>
    	<td></td>
    	<td></td>
	<td></td>
       	<td></td>
    	<td></td>
    </tr>
    <tr> 
    	<td> TAAT</td>
    	<td>arxiv'2022</td>
	<td> 39/RTX2080Ti</td>
        <td> 0.696</td>
    	<td> -</td>
    	<td> 0.560</td>
       	<td> 0.643</td>
    	<td> 0.735</td>
    	<td>0.416</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
 	<tr> 
    	<td> HMFT</td>
    	<td>CVPR'2022</td>
	<td> 30/GTXTitan</td>
        <td> 0.758</td>
    	<td> -</td>
    	<td> 0.627</td>
       	<td> 0.553</td>
    	<td> 0.760</td>
    	<td>0.347</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
<tr> 
    	<td> TFNet</td>
    	<td>TCSVT'2022</td>
	<td>20</td>
    	<td></td>
    	<td></td>
    	<td></td>
    	<td>59.4</td>
    	<td>46.2</td>
    	<td>28.8</td>
    	<td></td>
    	<td></td>
    	<td></td>
    </tr>
    	<tr> 
    	<td> JMMAC</td>
    	<td>TIP'2021</td>
	<td> 4/RTX2080Ti</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> 0.665</td>
    	<td> 0.821</td>
    	<td>0.483</td>
        <td> 0.662</td>
    	<td> 0.818</td>
    	<td> 0.420</td>
    </tr>
      	<tr> 
    	<td> MANet++</td>
    	<td>TIP'2021</td>
	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> 0.509</td>
    	<td> 0.538</td>
    	<td>0.272</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
        <tr> 
    	<td>FANet</td>
    	<td>TIV'2021</td>
	<td> 19/RTX2080Ti</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> 0.472</td>
    	<td> 0.508</td>
    	<td>0.247</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
         <tr> 
    	<td> ADRNet</td>
    	<td>IJCV'2021</td>
	<td> 25/RTX2080Ti</td>
        <td> 0.622</td>
    	<td> -</td>
    	<td> 0.466</td>
       	<td> 0.622</td>
    	<td> 0.766</td>
    	<td>0.396</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
            <tr> 
    	<td> SiamCDA</td>
    	<td>TCSVT'2021</td>
	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> 0.682</td>
    	<td> 0.757</td>
    	<td>0.424</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
	<tr> 
    	<td> MaCNet</td>
    	<td> Sensors'2020</td>
	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> 0.545</td>
    	<td> 0.591</td>
    	<td>0.305</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td> mfDiMP</td>
    	<td> ICCVW'2019</td>
	<td> 28/GTXTitan</td>
        <td> 0.673</td>
    	<td> -</td>
    	<td> 0.554</td>
       	<td> 0.602</td>
    	<td> 0.804</td>
    	<td> 0.388</td>
        <td> 0.638</td>
    	<td> 0.793</td>
    	<td> 0.380</td>
    </tr>
    <tr> 
    	<td> MANet </td>
    	<td> ICCVW'2019</td>
	<td> -</td>
        <td> 0.455</td>
    	<td> 0.383</td>
    	<td> 0.326</td>
       	<td> 0.582</td>
    	<td> 0.701</td>
    	<td> 0.346</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
      <tr> 
    	<td>DAPNet</td>
    	<td> ACM MM'2019</td>
	<td> -</td>
        <td> 0.431</td>
    	<td> 0.383</td>
    	<td> 0.314</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
       <tr> 
    	<td> DAFNet</td>
    	<td> ICCVW'2019</td>
	<td> -</td>
        <td> 0.620</td>
    	<td> -</td>
    	<td> 0.458</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td> FSRPN</td>
    	<td> 2019</td>
	<td> -</td>
        <td> 0.653</td>
    	<td> -</td>
    	<td> 0.544</td>
       	<td> -</td>
    	<td> -</td>
    	<td>0.355</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
            <tr> 
    	<td> SiamFT</td>
    	<td> IEEE Access'2019</td>
	<td> 30/RTX1080Ti</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> 0.630</td>
    	<td> 0.639</td>
    	<td>0.310</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
</table>

-----
## Methods

-----
## Competitions

 1. [AntiUAV 1st](https://anti-uav.github.io/)
	The first AntiUAV challenge is a multi-modal challenge. It was held in 2020.  The website for the 1st AntiUAV is covered by the newest one. The winner is team *xiaobaibai*. One of its member is [Tianyang Xu](https://xu-tianyang.github.io/)
 2. [VOT-RGBT2019](https://votchallenge.net/vot2019/)
 	The first competition in the RGBT tracking community. It was held in 2019. The winner is *SiamDW*.
 3. [VOT-RGBT2020]
    A competition in the RGBT tracking community. It was held in 2020. The winner is *DFAT*. One of its member is [Zhangyong Tang](https://github.com/Zhangyong-Tang/)

-----
## Contributors
- [Zhangyong Tang](https://github.com/Zhangyong_Tang)
- [PRCI-Lab](https://github.com/PRCI-Lab)

**Questions**

If you have any questions, please contact zhangyong_tang_jnu@163.com, and wechat: Tzy18861871359  is also welcomed.



 
