# Covid-19-Infection-Percentage-Estimation-Challenge:

Since the end of 2019, the World has faced a health crisis because of the COVID-19 pandemic. Infact, using Medical Imagings has proved their efficiency to detect Covid-19 Infection. These Medical Imagings inlude: X-ray, CT-scans and Ultrasound. Actually, the use of the CT scans is not only limited to the recognition of COVID-19 cases, but they can be used for other important tasks, which include quantifying the infection and monitoring the evolution of the disease, which can help with treatment and save the patient’s life. 
In this challenge, the competitors will use a dataset that were labelled by two expert radiologists who estimated the Covid-19  infection. In  the  testing  phase,  they  will  test  their  approach using two testing datasets, where the Covid-19 infection percentage were estimated after segmenting the Covid-19 infection and Lungs mask.


## Evaluation:

The evaluation metrics are:  Mean Absolute Error (MAE), Pearson Correla-tion coefficient (PC) and Root Mean Square Error (RMSE). The main Evaluation Criterion is the MAE of the Val set. In the case that two or more competitors achieve the same MAE, the PC and RMSE are considered as the tie-breaker, respectively. 

## Terms and Conditions:

1- The  competitors  are  asked  to  estimate  the  Covid-19  infection  percentage from each slice using deep learning techniques.  Only the pretrained models on ImageNet and Lung Nodules Segmentation are allowed. Using any external data or other pretrained models are not allowed.  The models must be trained using the training data and evaluated using the validation data.

2- Our dataset is only available for research purposes. When you use this dataset, you should give appropriate credit and not use the work for commercial purposes.
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

The challenge has three sets: Train, Val, and Test. The Train set is obtained from 132 CT-scans, from which 128 CT-scans has confirmed to have Covid-19 based on positive reverse transcription poly-merase chain reaction (RT-PCR) and CT scan manifestations identified by twoexperienced thoracic radiologists. The rest four CT-scans have not any infection type (Healthy). The Val set is obtained from 57 CT-scans, from which 55 CT-scans has confirmed to have Covid-19 based on positive reverse transcription poly-merase chain reaction (RT-PCR) and CT scan manifestations identified by twoexperienced thoracic radiologists. The rest  two CT-scans have not any infection type (Healthy). 

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


The test data contains two parts: 

- The details of the testing data will be released later.

  From each CT scan,  the radiologistspicked the slices that contain signs of COVID-19 infection and the ones that donot contain any COVID-19 signs.  The dataset were splitted into training andvalidation sets (70%, 30%), (132 Ct-scans, 57 Ct-scans).The test dataset contains two splits:•100 slices from 100 Ct-scans.•29 3D CT-scansThe  competitors  are  asked  to  estimate  the  Covid-19  infection  percentagefrom each slice using deep learning techniques.  Only the pretrained models onImageNet and Lung Nodules Segmentation are allowed. Using any external dataor other pretrained models are not allowed.  The models must be trained usingthe training data and evaluated using the validation data.The evaluation metrics are:  Mean Absolute Error (MAE), Pearson Correla-tion coefficient (PC) and Root Mean Square Error (RMSE).Since there are two evaluation datasets, the final performance will be calcu-lated as follow:MAEfinal= 0.3×MAE100slices+ 0.7×MAE29−3d−ctsP Cfinal= 0.3×P C100slices+ 0.7×P C29−3d−ctsRMSEfinal= 0.3×RMSE100slices+ 0.7×RMSE29−3d−ctsThe comparision between the teams results will be based onMAEfinal.  Iftwo or more teams got thte sameMAEfinal, theP Cfinalwill be used for thecomparison, thenRMSEfinal

## How to Participate:

You have to provide a single zip file that contains two files '.txt' file which has the name of the team and 'Val.csv', that contains the names of the slice images in the first column and their corresponding Covid-19 infection percentage in the second column. 
Similar to the training data, you have to provide a single zip containing a folder "sequences". The sequence folder contains sub-folders "11", "12", ..., "21", which contain a folder "predictions". There one has to provide for each scan a label file in binary format containing for each point an unsigned int (32-bit) with the label.
```bash
    Validation_phase.zip
    ├── Team_Name.txt 
    ├── Val.csv
    │      ├ Image_0000.png    Pr1            
    │      ├ Image_0001.png    Pr2             
    │      ├ ...               ...              
    │      └ Image_1342.png    Pr1342	        
    └──   
 ```   


## The competition schedules:
The challenge schedule will be as follow:

* 15/10/2021:  Train and Validation data release.

* 15/11/2021:  Testing datasets release.

* 30/11/2022:  Challenge ends.
 
* 10/12/2021:  Top 5 teams should send their packages that contain theircodes to be checked.
 
* 20/12/2021:  After checking the codes, the Top 5 teams will be notified tosend their papers.
 
* 15/01/2022:  deadline to submit their papers.
 
* 20/01/2022:  Papers reviewing ends.
