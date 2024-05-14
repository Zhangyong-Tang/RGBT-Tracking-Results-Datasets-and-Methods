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

## Datasets
***Real Data***

| Dataset | Publish  | GitHub| Introduction|
|--|--|--| --|
| GTOT | TIP'2016 | [GTOT](https://pan.baidu.com/s/1QNidEo-HepRaS6OIZr7-Cw) | 50 Video pairs, about 1.5W frames|
| RGBT210| ACM MM'2017 | [RGBT210](https://drive.google.com/file/d/0B3i2rdXLNbdUTkhsLVRwcTBTMlU/view?resourcekey=0-vytg_w3hqlQfLhoiS2J8Dg) | 210 Video pairs|
| RGBT234| PR'2018 | [RGBT234](https://sites.google.com/view/ahutracking001/)| 234 Video pairs, the extension of RGBT210 |
| VOT-RGBT19| VOT Community：2019 |[VOT-RGBT2019](https://pan.baidu.com/s/1kYnTTWF9LIkrCH4NNsSlFQ) *CODE:TZYD* | 60 Video pairs, about 2W frame pairs, a sub-set of RGBT 234|
| VOT-RGBT20|VOT Community： 2020 | [VOT-RGBT2020](https://pan.baidu.com/s/1fNgAVk4siqP2p-b1M2ZGmg ) *CODE:TZYD*| 60 Video pairs, its data is the same with VOT-RGBT2019, but with different evaluation mechanism|
| LasHeR| TIP'2021 | [LasHeR](https://github.com/BUGPLEASEOUT/LasHeR) | train/test split, imaged in the head-up view, above 70W image pairs in total; 245 videos in the test set|
| VTUAV| CVPR'2022 |[VTUAV](https://zhang-pengyu.github.io/DUT-VTUAV/) | imaged in the top-down view by uav, long-term;176 videos in the test-st, which has around 3500 frames in average|

***Generated Data***
| Dataset | Publish  | GitHub| Introduction|
|--|--|--| --|
| LSS-Dataset(from RGB) | TCSVT'2021 | [LSS-Dataset](https://pan.baidu.com/s/1x2hiqb2lSo54_4CI_L9YeQhttps://pan.baidu.com/s/1x2hiqb2lSo54_4CI_L9YeQ) ,code(Ye5Q)| Generated from VID|
| LSS-Dataset(from TIR) | TCSVT'2021 | [LSS-Dataset](https://pan.baidu.com/s/1xD3Ox-9VbZnyRQSWOxQRNw),code(IHws) | Generated from TIR|
-----
## Results


<table>
    <tr> 
        <th colspan="1"></th> 
        <th colspan="1"></th> 
	<th colspan="1"></th> 
	<th colspan="1"></th> 
        <th colspan="2">GTOT</th> 
        <th colspan="2">RGBT210</th> 
        <th colspan="2">RGBT234</th> 
        <th colspan="3">LasHeR</th> 
        <th colspan="3">VTUAV</th> 
        <th colspan="3">VOT-RGBT2019</th> 
        <th colspan="3">VOT-RGBT2020</th> 
    </tr>
    <tr>
    	<td> Methods</td>
    	 <td>Code</td>
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
    	<td> fusionnet</td>
    	    	<td> -</td>
    	<td> NeuroComputing'2018</td>
	<td> -</td>
    	<td> 0.852</td>
    	<td> 0.626</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td> mfDiMP</td>
    	    	<td> <a href='https://github.com/zhanglichao/end2end_rgbt_tracking'>pubished</a></td>
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
    	    	<td> <a href='https://github.com/Alexadlu/MANet'>pubished</a> </td>
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
    	<td> <a href='https://arxiv.org/pdf/1907.10451.pdf'>DAPNet</a></td>
    	    	<td> -</td>
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
    	    	<td> <a href='https://github.com/mjt1312/DAFNet'>pubished</a></td>
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
    	<td> -</td>
    	    	<td> -</td>
    	<td> ICIP'2019</td>
	<td> -</td>
    	<td> 0.843</td>
    	<td> 0.677</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.787</td>
    	<td> 0.545</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td> -</td>
    	    	<td> -</td>
    	<td> FUSION'2019</td>
	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.610</td>
    	<td> 0.428</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td> FSRPN</td>
    	    	<td> <a href='https://github.com/hli1221/rgbt-tracking-fsrpn'>published</a></td>
    	<td> 2019</td>
	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
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
    	<td>  <a href='https://ieeexplore.ieee.org/document/8809774'>SiamFT</a></td>
    	    	<td> -</td>
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
	<tr> 
    	<td> MaCNet</td>
    	    	<td> <a href='https://github.com/Lee-zl/MaCNet'>pubished</a></td>
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
    	<td>  <a href='https://openaccess.thecvf.com/content_CVPR_2020/papers/Wang_Cross-Modal_Pattern-Propagation_for_RGB-T_Tracking_CVPR_2020_paper.pdf'>CMPP</a></td>
    	    	<td> -</td>
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
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    	<tr> 
    	<td> <a href='https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123670222.pdf'>CAT</a></td>
    	    	<td> -</td>
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
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    	<tr> 
    	<td> <a href='https://www.sciencedirect.com/science/article/pii/S092359651930342X'>DSiamMFT</a></td>
    	    	<td> -</td>
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
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    	<tr> 
    	<td> JMMAC</td>
    	    	<td> <a href='https://github.com/zhang-pengyu/JMMAC'>pubished</a></td>
    	<td>TIP'2021</td>
	<td> 4/RTX2080Ti</td>
    	<td>0.902</td>
    	<td> 0.732</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.790</td>
    	<td> 0.573</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
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
    	<td> <a href='https://github.com/Alexadlu/MANet_pp'>MANet++</a></td>
    	    	<td> -</td>
    	<td>TIP'2021</td>
	<td> -</td>
    	<td>0.901</td>
    	<td> 0.723</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.800</td>
    	<td> 0.554</td>
    	<td> 0.467</td>
    	<td> 0.404</td>
    	<td> 0.314</td>
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
    	<td> <a href='https://ieeexplore.ieee.org/abstract/document/9340007'>CBPNet</a></td>
    	    	<td> -</td>
    	<td>TMM'2021</td>
	<td> -</td>
    	<td>0.885</td>
    	<td> 0.716</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.794</td>
    	<td> 0.541</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
       	<tr> 
    	<td>  <a href='https://pubmed.ncbi.nlm.nih.gov/34502691/'>CEDiMP</a></td>
    	    	<td> -</td>
    	<td>Sensors'2021</td>
	<td> -</td>
    	<td>0.886</td>
    	<td> 0.731</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.808</td>
    	<td> 0.561</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
       <tr> 
    	<td> <a href='https://ieeexplore.ieee.org/document/9383014'>TFNet</a></td>
    	    	<td> -</td>
    	<td>TCSVT'2021</td>
	<td> 20/RTX2080Ti</td>
    	<td>0.886</td>
    	<td> 0.729</td>
    	<td> 0.777</td>
    	<td> 0.529</td>
    	<td> 0.806</td>
    	<td> 0.560</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> 0.462</td>
    	<td> 0.594</td>
    	<td>0.288</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
        <tr> 
    	<td> <a href='https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=90354574'>FANet</a></td>
    	    	<td> -</td>
    	<td>TIV'2021</td>
	<td> 19/RTX2080Ti</td>
    	<td>0.891</td>
    	<td> 0.728</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.787</td>
    	<td> 0.553</td>
    	<td> 0.441</td>
    	<td> 0.384</td>
    	<td> 0.309</td>
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
    	    	<td> <a href='https://github.com/zhang-pengyu/ADRNet'>pubished</a></td>
    	<td>IJCV'2021</td>
	<td> 25/RTX2080Ti</td>
    	<td>0.904</td>
    	<td> 0.739</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.809</td>
    	<td> 0.571</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
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
    	<td> <a href='https://ieeexplore.ieee.org/document/9617143'>M^5L</a></td>
    	    	<td> -</td>
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
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
            <tr> 
    	<td> SiamCDA</td>
    	    	<td> <a href='https://github.com/Tianlu-Zhang/LSS-Dataset'> published </a> </td>
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
    	<td> <a href='https://link.springer.com/article/10.1007/s00371-021-02131-4'>DuSiamRT</a></td>
    	    	<td> -</td>
    	<td>2021</td>
	<td> -</td>
    	<td>0.766</td>
    	<td> 0.628</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.567</td>
    	<td> 0.384</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
   <tr> 
    	<td> <a href='https://www.sciencedirect.com/science/article/pii/S0925231221011966'>Here</a></td>
    	    	<td> -</td>
    	<td>NeuralComputing'2021</td>
	<td> 35</td>
    	<td>0.869</td>
    	<td> 0.711</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.751</td>
    	<td> 0.491</td>
    	<td> -</td>
    	<td> -</td>
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
    	<td> EStaple</td>
    	    	<td> -</td>
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
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td> APFNet</td>
    	    	<td> <a href='https://github.com/yangmengmeng1997/APFNet'> published </a> </td>
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
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    <tr> 
    	<td> TAAT</td>
    	    	<td> <a href='https://arxiv.org/abs/2201.08949'> arxiv </a> </td>
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
    	<td> <a href='https://pubmed.ncbi.nlm.nih.gov/35604973/'> DCNet </a></td>
    	    	<td> - </td>
    	<td>ICPR'2022</td>
	<td> -</td>
    	<td>0.903</td>
    	<td> 0.736</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.839</td>
    	<td> 0.591</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
 	<tr> 
    	<td> <a href='https://openaccess.thecvf.com/content_CVPR_2019/papers/Shou_DMC-Net_Generating_Discriminative_Motion_Cues_for_Fast_Compressed_Video_Action_CVPR_2019_paper.pdf'> DMCNet </a></td>
    	    	<td> -</td>
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
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
    </tr>
 	<tr> 
    	<td> MFGNet</td>
    	    	<td> <a href='https://github.com/wangxiao5791509/MFG_RGBT_Tracking_PyTorch'>pubished</a></td>
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
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
 	<tr> 
    	<td> HMFT</td>
    	    	<td> <a href='https://github.com/zhang-pengyu/HMFT'> published</a></td>
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
    	<td> <a href='https://link.springer.com/article/10.1007/s11432-020-3160-5'>Here</a></td>
    	<td> -</td>
    	<td>SC IF'2022</td>
	<td> 10/i5-7500k</td>
    	<td>0.864</td>
    	<td> 0.707</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.666</td>
    	<td> 0.484</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	 <td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
       <tr> 
    	<td> <a href='https://dl.acm.org/doi/10.1145/3503161.3547851'> ProTrack </a></td>
    	<td> -</td>
    	<td>ACMMM'2022</td>
	<td> -</td>
    	<td>-</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.786</td>
    	<td> 0.587</td>
    	<td> 0.509</td>
    	<td> -</td>
    	<td> 0.421</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	 <td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
       <tr> 
    	<td> DFAT</td>
    	<td> <a href='https://github.com/Zhangyong-Tang/DFAT-Information-Fusion/'>published</a></td>
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
    	<td> ViPT</td>
    	<td> <a href='https://github.com/jiawen-zhu/ViPT'>published</a></td>
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
        <td> -</td>
    	<td> -</td>
    	 <td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
       <tr> 
    	<td> <a href='[https://github.com/jiawen-zhu/ViPT](https://eprints.whiterose.ac.uk/198539/1/4808_efficient_rgb_t_tracking_via_c-Camera-ready%20PDF.pdf)'>HFRD</a></td>
    	<td> -</td>
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
        <td> -</td>
    	<td> -</td>
    	 <td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
       <tr> 
    	<td> TBSI</td>
    	<td> <a href='https://github.com/RyanHTR/TBSI'>published</a></td>
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
        <td> -</td>
    	<td> -</td>
    	 <td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
       <tr> 
    	<td> <a href='https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10184056'>BD2Track</a></td>
    	<td> -</td>
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
        <td> -</td>
    	<td> -</td>
    	 <td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
       <tr> 
    	<td> <a href='https://ieeexplore.ieee.org/document/10226308'>SiamTDR</a></td>
    	<td> -</td>
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
        <td> -</td>
    	<td> -</td>
    	 <td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
       <tr> 
    	<td>  <a href='https://pubmed.ncbi.nlm.nih.gov/37587133/'>SiamAFTS</a> </td>
    	<td> -</td>
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
        <td> -</td>
    	<td> -</td>
    	 <td> -</td>
    	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td><a href='https://link.springer.com/article/10.1007/s10489-023-04741-y'>paper</a> </td>
    	<td> -</td>
    	<td>Applied Intelligence'2023</td>
	<td> 15/GTX1080Ti</td>
    	<td>91.6</td>
    	<td> 74.4</td>
    	<td> 80.2</td>
    	<td> 56.8</td>
    	<td> 83.6</td>
    	<td> 60.4</td>
	<td> 63.6</td>
       	<td> 59.4</td>
    	<td> 50.0</td>
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
    	<td>UMT</td>
    	<td> -</td>
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
    	<td> </td>
    	<td> -</td>
    	<td> </td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	
<!-- <tr>  -->
<!--     	<td> <a href='https://arxiv.org/abs/2308.13764'>USTrack</a></td>
    	<td> -</td>
    	<td>Arxiv'2023</td>
	<td> 84.2/RTX3090</td>
    	<td>93.4</td>
    	<td> 78.3</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 87.4</td>
    	<td> 65.8</td>
	<td> -</td>
       	<td> -</td>
    	<td> -</td>
    	<td> 86.9</td>
    	<td> -</td>
    	<td> 74.4</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr> -->
<tr> 
    	<td> <a href='https://ieeexplore.ieee.org/abstract/document/10252033'>RFSTrack</a></td>
    	<td> -</td>
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
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
<tr> 
    	<td> <a href='https://dl.acm.org/doi/10.1145/3581783.3612341'>QAT</a></td>
    	<td> -</td>
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
    	<td><a href='https://github.com/SparkTempest/BAT'>BAT</a></td>
    	<td> -</td>
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
    	<td> </td>
    	<td> -</td>
    	<td> </td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
    </tr>
	 <tr> 
    	<td><a href='https://arxiv.org/abs/2401.01244'>TATrack</a></td>
    	<td> -</td>
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
    	<td> </td>
    	<td> -</td>
    	<td> </td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td> <a href='https://github.com/Zhangyong-Tang/GMMT'>GMMT</a></td>
    	<td> -</td>
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
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td> <a href='https://github.com/mjt1312/Lminet'>(47th) LMINet</a></td>
    	<td> -</td>
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
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td> <a href='https://ieeexplore.ieee.org/abstract/document/10460420'>CAT++</a></td>
    	<td> -</td>
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
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td> <a href='https://ieeexplore.ieee.org/abstract/document/10472533'>AMNet</a></td>
    	<td> -</td>
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
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td> <a href='https://ieeexplore.ieee.org/abstract/document/10516307?casa_token=jEMySzd_jh0AAAAA:2EFbV9i_xl8yQM8i0tUlZKVk9RMcOn45MbxiKouZjIQ3RDR7mVK8LeA3MVCBzWOlkDIBQL2W79c'>QueryTrack</a></td>
    	<td> -</td>
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
    	<td> <a href='https://ieeexplore.ieee.org/abstract/document/10517645'>MCTrack</a></td>
    	<td> -</td>
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
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td> <a href='https://arxiv.org/abs/2403.16002'>SDSTrack</a></td>
    	<td> <a href='hhttps://github.com/hoqolo/SDSTrack'>publshed</a></td>
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
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td> <a href='https://arxiv.org/abs/2403.09634'>OneTracker</a></td>
    	<td> -</td>
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
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td> <a href='https://github.com/Zongwei97/UnTrack'>UnTrack</a></td>
    	<td> -</td>
    	<td>CVPR'2024</td>
	<td> -</td>
    	<td>-</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 84.2</td>
    	<td> 62.5</td>
	<td> -</td>
       	<td> 66.7</td>
    	<td> 53.6</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    	<td>-</td>
        <td> -</td>
    	<td> -</td>
    </tr>
	 <tr> 
    	<td> <a href='https://arxiv.org/abs/2405.02717'>AFter</a></td>
    	<td> -</td>
    	<td>Arxiv'2024</td>
	<td>RTX 4090/23</td>
    	<td>91.6</td>
    	<td> 78.5</td>
    	<td> 87.6</td>
    	<td> 63.5</td>
    	<td> 90.1</td>
    	<td> 66.7</td>
	<td> 70.3</td>
       	<td> 65.8</td>
    	<td> 55.1</td>
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



 
