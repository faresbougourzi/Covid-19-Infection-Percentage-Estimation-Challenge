# Covid-19-Infection-Percentage-Estimation-Challenge:

Since late 2019, the world been in health crisis because of the COVID-19 pandemic. In fact, using Medical Imagery has proved to be efficient in detecting Covid-19 Infection. These Medical Imaging inlude: X-ray, CT-scans and Ultrasounds. The use of CT-scans is not only limited to the detection of COVID-19 cases, but they can also be used for other important tasks such quantifying the infection and monitoring the evolution of the disease, which can help in treatment and save the patient’s life. 
In this challenge, the participants will use a dataset labelled by two expert radiologists, who estimated the Covid-19 infection, to train and valiadate their approaches. In  the  testing  phase,  participants  will  test  their  approaches a test dataset collected from various CT-scanners and recording settings. 

<!-- where the Covid-19 infection percentage were estimated after segmenting the Covid-19 infection and Lungs mask. -->

## The competition schedules:
The challenge schedule will be as follow:

* 01/12/2021:  Train and Validation data release. 

* 25/12/2021:  Testing datasets release.

* 31/12/2021:  The submission of the testing predictions deadline.
 
* 10/01/2022:  Top 5 teams should send their packages that contain their codes to be checked.
 
* 20/01/2022:  After checking the codes, the Top 5 teams will be notified to send their papers.
 
* 10/02/2022:  deadline to submit their papers.
 
* 20/02/2022:  Papers reviewing ends.

## The Organizers

* Fares Bougourzi, Dr, Institute of Applied Sciences and Intelligent Systems, National Research Council of Italy, 73100 Lecce, Italy

* Cosimo Distante, Pr, Institute of Applied Sciences and Intelligent Systems, National Research Council of Italy, 73100 Lecce, Italy

* Abdelmalik Taleb-Ahmed, Pr, Univ. Polytechnique Hauts-de-France, Univ. Lille, CNRS, Centrale Lille,  UMR 8520 - IEMN,  F-59313 Valenciennes, France

* Fadi Dornaika, Pr, University of the Basque Country UPV/EHU, San Sebastian, Spain; IKERBASQUE, Basque Foundation for Science, Bilbao, Spain

* Abdenour Hadid, Pr, Univ. Polytechnique Hauts-de-France, Univ. Lille, CNRS, Centrale Lille,  UMR 8520 - IEMN,  F-59313 Valenciennes, France


## Evaluation:

The evaluation metrics are:  Mean Absolute Error (MAE), Pearson Correla-tion coefficient (PC) and Root Mean Square Error (RMSE). The most important Evaluation Criterion is the MAE. In the event of two or more competitors achieve the same MAE, the PC and the RMSE are considered as the tie-breaker. 

## Terms and Conditions:

1- Team size: Teams should have at least 2 people and no more than 7 members.

2- Open Source. The workflow, codes, and presentations prepared as part of the competition will be released as open source.

3- The  competitors  are  asked  to  estimate  the  Covid-19  infection  percentage from each slice using Machine Learning.  Only the pretrained models on ImageNet and Lung Nodules Segmentation models are allowed. Using any external data or other pretrained models are not allowed.  The models must be trained using the training data and evaluated using the validation data.

4- Our dataset is only available for research purposes. When you use this dataset, you should give appropriate credit and not use the work for commercial purposes.
Specifically you should cite our work:
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

## Challenge Dataset:

The challenge has three sets: Train, Val, and Test. The Train set is obtained from 132 CT-scans, from which 128 CT-scans has confirmed to have Covid-19 based on positive reverse transcription poly-merase chain reaction (RT-PCR) and CT scan manifestations identified by twoexperienced thoracic radiologists. The rest four CT-scans have not any infection type (Healthy). The Val set is obtained from 57 CT-scans, from which 55 CT-scans has confirmed to have Covid-19 based on positive reverse transcription poly-merase chain reaction (RT-PCR) and CT scan manifestations identified by two experienced thoracic radiologists. The rest  two CT-scans have not any infection type (Healthy). 

Both Train and Val splits will two files: Images (Slices) Folder and Labeling Folder ('.csv' file) that contains the labels for each Slice (Image)
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
    │         └ Image_3011.png    49.0	               131
    └── 
    
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
    │         └ Image_1342.png    8.0	               56
    └──     

```

- The details of the testing data will be released later.


## Challenge Phases:

1- Validation Phase: The training and validation phase will be carried out in CodaLab plateform. For the validation set, each team has the possibility to send 10 predictions per day in CodaLab.
In the end of the validation phase, the Top-10 teams results on the validation data can participate in the Testing phase.

2- Testing Phase: In the testing phase, the Top-10 teams from validation phase will test their approaches using the testing data and submit their predictions, which will be evaluated then the final results will be released.


## How to Participate:

- Participation in the Competetion: Each team should request to participate in the competition on the CodaLab platform (https://competitions.codalab.org/competitions/35575) with specifying the team name, members, emails and affiliations. The team informations can be send to: faresbougourzi@gmail.com

- Validation Phase: You have to submit the predictions of the validation data as 'predictions.csv' file, that contains the names of the slice images in the first column and their corresponding Covid-19 infection percentage estimation in the second column.  This file must be compressed as 'predictions.zip' file and submitted in CodaLab. 

```bash
    predictions.zip
    ├── predictions.csv
    │      ├ Image_0000.png    Pr1            
    │      ├ Image_0001.png    Pr2             
    │      ├ ...               ...              
    │      └ Image_1342.png    Pr1342	        
    └──   
 ```   
 - In the Testing Phase: You have to submit the predictions of the validation data as 'Team_Name.csv' file, that contains the names of the slice images in the first column and their corresponding Covid-19 infection percentage estimation in the second column.  This file must be compressed as 'predictions.zip' file and submitted to the indicated adress email in the testing phase.
```bash
    Team_Name.zip
    ├── predictions.csv
    │      ├ Image_0000.png    Pr1            
    │      ├ Image_0001.png    Pr2             
    │      ├ ...               ...              
    │      └ Image_N.png       PrN        
    └──   
 ```   
 
 - The Top-5 teams are encaraged to submit a conference paper (Summurise the approach and diffent experiements) to our Workshop of Covid-19 in the 21st International Conference on IMAGE ANALYSIS AND PROCESSING (https://www.iciap2021.org/). Otherwise, you need to send us the link of the description approach in ARXIV paper.
 
## Prices:

The details about the Prices will be released later.

