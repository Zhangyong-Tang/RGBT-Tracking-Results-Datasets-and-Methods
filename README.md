## Deep-RGBT-Tracking-Results-Datasets-and-Methods

**This is a personal survey of the RGBT tracking community. 
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

| Dataset | Publish  | GitHub|
|--|--|--|
| GTOT | TIP'2016 | [GTOT](https://pan.baidu.com/s/1QNidEo-HepRaS6OIZr7-Cw) |
| RGBT210| ACM MM'2017 | [RGBT210](https://drive.google.com/file/d/0B3i2rdXLNbdUTkhsLVRwcTBTMlU/view?resourcekey=0-vytg_w3hqlQfLhoiS2J8Dg) |
| RGBT234| PR'2018 | [RGBT234](https://sites.google.com/view/ahutracking001/)|
| VOT-RGBT19| VOT Community：2019 |[VOT-RGBT2019](https://pan.baidu.com/s/1kYnTTWF9LIkrCH4NNsSlFQ) *CODE:TZYD* |
| VOT-RGBT20|VOT Community： 2020 | [VOT-RGBT2020](https://pan.baidu.com/s/1fNgAVk4siqP2p-b1M2ZGmg ) *CODE:TZYD*|
| LasHeR| TIP'2021 | [LasHeR](https://github.com/BUGPLEASEOUT/LasHeR) |
| VTUAV| CVPR'2022 |[VTUAV](https://zhang-pengyu.github.io/DUT-VTUAV/) |

-----
## Results

<table>
    <tr> 
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
    	    	<td> -</td>
    	<td> ICCVW'2019</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.786</td>
    	<td> 0.555</td>
    	<td> 0.785</td>
    	<td> 0.559</td>
    	<td> 0.447</td>
    	<td> -</td>
    	<td> 0.344</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> 0.602</td>
    	<td> 0.804</td>
    	<td> 0.388</td>
        <td> 0.638</td>
    	<td> 0.793</td>
    	<td> 0.380</td>
    </tr>
    <tr> 
    	<td> MANet </td>
    	    	<td> -</td>
    	<td> ICCVW'2019</td>
    	<td> 0.894</td>
    	<td> 0.724</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.777</td>
    	<td> 0.539</td>
    	<td> 0.457</td>
    	<td> -</td>
    	<td> 0.330</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> 0.582</td>
    	<td> 0.701</td>
    	<td> 0.346</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
      <tr> 
    	<td> DAPNet</td>
    	    	<td> -</td>
    	<td> ACM MM'2019</td>
    	<td> 0.882</td>
    	<td> 0.707</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.766</td>
    	<td> 0.537</td>
    	<td> 0.431</td>
    	<td> -</td>
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
    	<td> DAFNet</td>
    	    	<td> -</td>
    	<td> ICCVW'2019</td>
    	<td> 0.891</td>
    	<td> 0.712</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.796</td>
    	<td> 0.544</td>
    	<td> 0.449</td>
    	<td> -</td>
    	<td> 0.311</td>
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
    	<td> ICIP'2019</td>
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
    	<td> -</td>
    	    	<td> -</td>
    	<td> FUSION'2019</td>
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
    	<td> SiamFT</td>
    	    	<td> -</td>
    	<td> IEEE Access'2019</td>
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
    	    	<td> -</td>
    	<td> Sensors'2020</td>
    	<td>0.880</td>
    	<td> 0.714</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.790</td>
    	<td> 0.554</td>
    	<td> 0.483</td>
    	<td> -</td>
    	<td> 0.352</td>
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
    	<td> DMCNet</td>
    	    	<td> -</td>
    	<td></td>
    	<td>0.909</td>
    	<td> 0.733</td>
    	<td> 0.797</td>
    	<td> 0.555</td>
    	<td> 0.839</td>
    	<td> 0.593</td>
    	<td> 0.491</td>
    	<td> -</td>
    	<td> 0.357</td>
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
    	<td> CMPP</td>
    	    	<td> -</td>
    	<td>CVPR'2020</td>
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
    	<td> CAT</td>
    	    	<td> -</td>
    	<td>ECCV'2020</td>
    	<td>0.889</td>
    	<td> 0.717</td>
    	<td> 0.792</td>
    	<td> 0.533</td>
    	<td> 0.804</td>
    	<td> 0.561</td>
    	<td> 0.451</td>
    	<td> -</td>
    	<td> 0.317</td>
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
    	<td> DSiamMFT</td>
    	    	<td> -</td>
    	<td>2020</td>
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
    	    	<td> -</td>
    	<td>TIP'2021</td>
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
    	<td> MANet++</td>
    	    	<td> -</td>
    	<td>TIP'2021</td>
    	<td>0.901</td>
    	<td> 0.723</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.800</td>
    	<td> 0.554</td>
    	<td> 0.467</td>
    	<td> -</td>
    	<td> 0.317</td>
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
    	<td> CBPNet</td>
    	    	<td> -</td>
    	<td>TMM'2021</td>
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
    	<td> TFNet</td>
    	    	<td> -</td>
    	<td>TCSVT'2021</td>
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
    	<td> FANet</td>
    	    	<td> -</td>
    	<td>TIV'2021</td>
    	<td>0.891</td>
    	<td> 0.728</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.787</td>
    	<td> 0.553</td>
    	<td> 0.442</td>
    	<td> -</td>
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
    	    	<td> -</td>
    	<td>IJCV'2021</td>
    	<td>0.904</td>
    	<td> 0.739</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.809</td>
    	<td> 0.571</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> 0.622</td>
    	<td> 0.766</td>
    	<td>0.396</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
          <tr> 
    	<td> ADRNet</td>
    	    	<td> -</td>
    	<td>IJCV'2021</td>
    	<td>0.904</td>
    	<td> 0.739</td>
    	<td> -</td>
    	<td> -</td>
    	<td> 0.809</td>
    	<td> 0.571</td>
    	<td> -</td>
    	<td> -</td>
    	<td> -</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
       	<td> 0.622</td>
    	<td> 0.766</td>
    	<td>0.396</td>
        <td> -</td>
    	<td> -</td>
    	<td> -</td>
    </tr>
           <tr> 
    	<td> M^5L</td>
    	    	<td> -</td>
    	<td>TIP'2021</td>
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
    	    	<td> -</td>
    	<td>TCSVT'2021</td>
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
    	<td> DuSiamRT</td>
    	    	<td> -</td>
    	<td>2021</td>
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
    	<td> APFNet</td>
    	    	<td> -</td>
    	<td>AAAI'2022</td>
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
    	<td> DFAT</td>
    	    	<td> <a herf="https://github.com/Zhangyong-Tang/DFAT-Information-Fusion">published</a></td>
    	<td>INFFUS'2023</td>
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



 
