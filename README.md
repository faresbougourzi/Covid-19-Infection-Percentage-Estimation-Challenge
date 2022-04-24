# Covid-19-Infection-Percentage-Estimation-Challenge:

## Chanllenge Plateform (CodaLab):
https://competitions.codalab.org/competitions/35575

## Overview:
Since late 2019, the world been in health crisis because of the COVID-19 pandemic. In fact, using Medical Imagery has proved to be efficient in detecting Covid-19 Infection. These Medical Imaging include: X-ray, CT-scans and Ultrasounds. The use of CT-scans is not only limited to the detection of COVID-19 cases, but they can also be used for other important tasks such quantifying the infection and monitoring the evolution of the disease, which can help in treatment and save the patient’s life. 
In this challenge, the participants will use a dataset labelled by two expert radiologists, who estimated the Covid-19 infection, to train and validate their approaches. In  the  testing  phase,  participants  will  test  their  approaches using a test dataset collected from various CT-scanners and recording settings. 

<!-- where the Covid-19 infection percentage were estimated after segmenting the Covid-19 infection and Lungs mask. -->

## The Competition Schedules:
The challenge schedule will be as follow:

* 	16/10/2021: The competition Starts. Train and Validation data will be released. :heavy_check_mark:
 	
*	20/12/2021: Testing datasets release.  :heavy_check_mark:
	
* 30/12/2021: Deadline to submit the testing predictions.   :heavy_check_mark:

* 30/01/2022: Testing Rank release. The Top-teams should submit their packages (that contain their codes to be checked; better to provide github link), and their approach's description text, it is prefered to submit an the ARXIV link (but you can submit a PDF as well)  :heavy_check_mark:
 

*   15/03/2022: Deadline to submit the papers to the associated Covid-19 Workshop,  https://sites.google.com/view/covid19iciap2022/.  :heavy_check_mark:

## The Competition Ranking:
### The Winning Teams
1- Suman Chaudhary and  Wanting Yang

2- Talha Anwar

3- Radu Miron, Cosmin Moisii, Vlad Barbu and Mihaela Breaban

4- Chih-Chung Hsu, Sheng-Jay Tai, and Shao-Min Chen

5- Davide Tricarico, Ayesha Chaudhry, Attilio Fiandrotti, and Marco Grangetto

6- Maria Ausilia Napoli Spatafora, Sebastiano Battiato, Alessandro Ortis, and Daniela Campisi.

### Validation Results			
|Team Name |             	Codalab Username| 	MAE|	PC| 	RMSE|
|:--------|:----------|:---------|:----------|:---------|
|1.SenticLab.UAIC| 	SenticLab.UAIC|	4.17140661|	0.948787386|	8.196144648|
|2.TAC|	talhaanwar|	4.484023556|	0.946005946|	8.547415523|
|3.Taiyuan_university_lab713| 	suman|	4.504261529|	0.949030574|	8.096456422|
|4.EIDOSlab_Unito| 	davide.tricarico|	4.912411698|	0.942962971|	8.700152227|
|5.ausilianapoli94|	ausilianapoli94|	4.95311299|	0.943508386|	8.603844126|
|6.ACVLab|	 ACVLab|	4.992599789|	0.9364718|	9.080638078|
				
				
### Testing Results				
|Team Name              	|Codalab Username| 	MAE|	PC| 	RMSE|
|:--------|:----------|:---------|:----------|:---------|
|1.Taiyuan_university_lab713|	suman|	3.556981966|	0.854795953|	7.51020585|
|2.TAC|	talhaanwar|	3.645392997|	0.802208221|	8.570867077|
|3.SenticLab.UAIC|	SenticLab.UAIC|	4.617217352|	0.7634996|	9.099633322|
|4.ACVLab|	ACVLab|	4.866063832|	0.72872904|	10.27505977|
|5.EIDOSlab_Unito|	davide.tricarico|	5.020207858|	0.797797023|	9.005695703|
|6.IPLab|	ausilianapoli94|	6.536300292|	0.709168691|	9.97612344|
				


### Final Ranking  (0.3 Val+0.7 Test)	
|Team Name              	|Codalab Username| 	MAE|	PC| 	RMSE|
|:--------|:----------|:---------|:----------|:---------|
|1.Taiyuan_university_lab713|	suman|	3.8411658349|	0.8830663393|	7.920581250|
|2.TAC|	talhaanwar|	3.8969821647|	0.8453475385| 	8.5544509892|
|3.SenticLab.UAIC| 	SenticLab.UAIC|	4.4834741293|	0.81908593579|	8.4671912502|
|4.ACVLab| 	ACVLab|	4.904024619|	0.791051868|	9.43896458559|
|5.EIDOSlab_Unito|	davide.tricarico|	4.98786901| 	0.8413468073| 	8.7918152698|
|6.IPLab|	ausilianapoli94|	6.06134410|	0.7794705995|	9.0155279202|


<!---
### Testing Results				
|Team Name              	|Codalab Username| 	MAE|	PC| 	RMSE|
|:--------|:----------|:---------|:----------|:---------|
|1.Taiyuan_university_lab713|	suman|	3.556981966|	0.854795953|	7.51020585|
|2.TAC|	talhaanwar|	3.645392997|	0.802208221|	8.570867077|
|3.SenticLab.UAIC|	SenticLab.UAIC|	4.617217352|	0.7634996|	9.099633322|
|4.ACVLab|	ACVLab|	4.866063832|	0.72872904|	10.27505977|
|5.EIDOSlab_Unito|	davide.tricarico|	5.020207858|	0.797797023|	9.005695703|
|6.IPLab|	ausilianapoli94|	6.536300292|	0.709168691|	9.97612344|

 
* 01/12/2021:  Train and Validation data release. 

* 25/12/2021:  Testing datasets release.

* 31/12/2021:  The submission of the testing predictions deadline.
 
* 10/01/2022:  Top 5 teams should send their packages that contain their codes to be checked.
 
* 20/01/2022:  After checking the codes, the Top 5 teams will be notified to send their papers.
 
* 10/02/2022:  Deadline to submit their papers.
 
* 20/02/2022:  Papers reviewing ends. 
 https://drive.google.com/file/d/1BaLg5c_vjoVMU6eBNDTRnBzIV04RyGGd/view?usp=sharing
--->

## The Organizers

* Fares Bougourzi, Dr, Institute of Applied Sciences and Intelligent Systems, National Research Council of Italy, 73100 Lecce, Italy

* Cosimo Distante, Pr, Institute of Applied Sciences and Intelligent Systems, National Research Council of Italy, 73100 Lecce, Italy

* Abdelmalik Taleb-Ahmed, Pr, Univ. Polytechnique Hauts-de-France, Univ. Lille, CNRS, Centrale Lille,  UMR 8520 - IEMN,  F-59313 Valenciennes, France

* Fadi Dornaika, Pr, University of the Basque Country UPV/EHU, San Sebastian, Spain; IKERBASQUE, Basque Foundation for Science, Bilbao, Spain

* Abdenour Hadid, Pr, Univ. Polytechnique Hauts-de-France, Univ. Lille, CNRS, Centrale Lille,  UMR 8520 - IEMN,  F-59313 Valenciennes, France


## Evaluation:

The evaluation metrics are:  Mean Absolute Error (MAE), Pearson Correlation coefficient (PC) and Root Mean Square Error (RMSE). The most important Evaluation Criterion is the MAE. In the event of two or more competitors achieve the same MAE, the PC and the RMSE are considered as the tie-breaker. 

## Terms and Conditions:

1- Team size: Teams should consist of a minimum of 2  and maximum of 7 members.

2- Open Source: The workflow, codes, and presentations created as part of the competition will be as open source.

3- General Rules: Participants  should  estimate  the  percentage of Covid-19  infection  from each slice using Machine Learning.  Only  ImageNet's pre-trained models and Lung Nodule Segmentation models are allowed. The use of external data or other pre-trained models is not allowed.  The models must be trained using the training data and evaluated using the validation data.

4- Citation: The provided dataset is available for research purposes only. If you use this dataset, you should cite it appropriately and not use the work for commercial purposes. 
In particular, you should cite the following works:
```bash
@Article{jimaging7090189,
AUTHOR = {Bougourzi, Fares and Distante, Cosimo and Ouafi, Abdelkrim and Dornaika, Fadi and Hadid, Abdenour and Taleb-Ahmed, Abdelmalik},
TITLE = {Per-COVID-19: A Benchmark Dataset for COVID-19 Percentage Estimation from CT-Scans},
JOURNAL = {Journal of Imaging},
VOLUME = {7},
YEAR = {2021},
NUMBER = {9},
ARTICLE-NUMBER = {189},
URL = {https://www.mdpi.com/2313-433X/7/9/189},
ISSN = {2313-433X},
DOI = {10.3390/jimaging7090189}
}
```
```bash
@article{vantaggiato2021covid,
  title={Covid-19 recognition using ensemble-cnns in two new chest x-ray databases},
  author={Vantaggiato, Edoardo and Paladini, Emanuela and Bougourzi, Fares and Distante, Cosimo and Hadid, Abdenour and Taleb-Ahmed, Abdelmalik},
  journal={Sensors},
  volume={21},
  number={5},
  pages={1742},
  year={2021},
  publisher={Multidisciplinary Digital Publishing Institute}
}
```

## Challenge Dataset:

The challenge has three sets: Train, Val, and Test. The Train set is obtained from 132 CT-scans, from which 128 CT-scans has confirmed to have Covid-19 based on positive reverse transcription polymerase chain reaction (RT-PCR) and CT scan manifestations identified by two experienced thoracic radiologists. The rest four CT-scans have not any infection type (Healthy). The Val set is obtained from 57 CT-scans, from which 55 CT-scans has confirmed to have Covid-19 based on positive reverse transcription polymerase chain reaction (RT-PCR) and CT scan manifestations identified by two experienced thoracic radiologists. The rest  two CT-scans have not any infection type (Healthy). 

The Train split has two files: Images (Slices) Folder and Labeling Folder ('.csv' file) that contains the labels for each Slice (Image)

The Train Split can be downloaded from the link:

https://drive.google.com/drive/folders/1vPYMrL_IwC_wOxff3wX_Rg1iIJyNl2Dc?usp=sharing
```bash
    Train Set
    ├── Slices Folder 
    │      ├ Image_0000.png
    │      ├ Image_0001.png
    │      ├ ...
    |      └ Image_3011.png
    ├── Labeling Folder
    │   └── Train.csv
    │         ├ Slice_Name        Covid-19_percentage  Subject    
    │         ├ Image_0000.png    0.0                  0
    │         ├ Image_0001.png    0.0                  0
    │         ├ ...               ...                  ..
    │         └ Image_3053.png    49.0	               131
    └── 
 ```   
    
    
The Validation split has one file contains the slices images, which will be used to predict the Covid-19 infection percentage. These prediction should be saved as '.csv' file and submitted to the Codalab (https://competitions.codalab.org/competitions/35575) to evaluation the performance:

The Validation Split can be downloaded from the link:

https://drive.google.com/drive/folders/18V_u6Vo75a_A5RlUH80UcXh3i0rc5keE?usp=sharing

```bash    
    Val Set
    ├── Slices Folder 
    │      ├ Image_0000.png
    │      ├ Image_0001.png
    │      ├ ...
    |      └ Image_1342.png
    ├── Labeling Folder
    │   └── Val.csv
    │         ├ Slice_Name        Covid-19_percentage  Subject    
    │         ├ Image_0000.png    0.0                  0
    │         ├ Image_0001.png    0.0                  0
    │         ├ ...               ...                  ..
    │         └ Image_1300.png    8.0	               56
    └──     

```

- The details of the testing data will be released later.


## Challenge Phases:

1- Validation Phase: The training and validation phase will be carried out in CodaLab platform. For the validation set, each team has the possibility to send five predictions per day in CodaLab.
In the end of the validation phase, the Top-10 teams results on the validation data can participate in the Testing phase.

2- Testing Phase: In the testing phase, the Top-10 teams from validation phase will test their approaches using the testing data and submit their predictions, which will be evaluated then the final ranking will be released.


## How to Participate:

- Participation in the Competition: Each team should request to participate in the competition on the CodaLab platform (https://competitions.codalab.org/competitions/35575) with specifying the team name, members, emails and affiliations. The team informations can be send to: faresbougourzi@gmail.com

- Validation Phase: In the Validation phase, each team should submit the predictions of the validation data as 'predictions.csv' file, which contains the names of the slice images in the first column and the corresponding Covid-19 infection percentage estimation in the second column.  This file should be compressed as 'predictions.zip' file and submitted to CodaLab. 

```bash
    predictions.zip
    ├── predictions.csv
    │      ├ Image_0000.png    Pr0            
    │      ├ Image_0001.png    Pr1             
    │      ├ ...               ...              
    │      └ Image_1300.png    Pr1300	        
    └──   
 ```   
 - Testing Phase: each team should submit the predictions of the Testing data as 'Team_Name.csv' file, that contains the names of the slice images in the first column and the corresponding Covid-19 infection percentage estimation in the second column.  This file must be compressed as 'predictions.zip' file and sent to: faresbougourzi@gmail.com.
```bash
    Team_Name.zip
    ├── predictions.csv
    │      ├ Image_0000.png    Pr1            
    │      ├ Image_0001.png    Pr2             
    │      ├ ...               ...              
    │      └ Image_N.png       PrN        
    └──   
 ```   
 
 - The Top-5 teams are encouraged to submit a conference paper (Summarize the approach and different experiments) to MIA COVID 2022 Workshop (https://sites.google.com/view/covid19iciap2022) in the 21st International Conference on IMAGE ANALYSIS AND PROCESSING (https://www.iciap2021.org/call-for-competitions-2/). otherwise, send us the ARXIV link.
 
## Prizes:

- The Winner team will be awarded with 500 Euros.

