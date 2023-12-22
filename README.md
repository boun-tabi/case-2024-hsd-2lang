# Hate Speech Detection in Turkish and Arabic Tweets (HSD-2Lang)
## Overview

Hate speech, which targets groups based on characteristics such as ethnicity, nationality, religion, colour, gender, and sexual orientation, is a significant problem on social media platforms. Automated detection of such content is crucial for effective content moderation and minimising societal harm, and can also be used in socio-political event analysis. 

The effectiveness of current hate speech detection models is often hampered by issues such as limited data and lack of generalizability. Following the [SIU2023-NST](https://myweb.sabanciuniv.edu/berrin/siu2023-nst/) competition organized to benchmark progress in Turkish hate speech detection and classification, we are organizing a new shared task in conjunction with [CASE @ EACL 2024](https://emw.ku.edu.tr/case-2024/). This shared task focuses on tackling the challenge of identifying hate speech in tweets in Turkish and Arabic languages. Participants will develop models to detect hate speech on a range of topics.

The task is divided into two subtasks:

A) Hate Speech Detection in Turkish across Various Contexts

B) Hate Speech Detection with Limited Data in Arabic

## Task Definitions
Participants will engage in binary classification tasks, determining whether individual tweets are hateful or non-hateful.
### Subtask A: Hate Speech Detection in Turkish across Various Contexts

- **Objective:** To develop a model capable of detecting hate speech in Turkish tweets.

- **Data:** The dataset contains a variety of Turkish tweets, each annotated for the presence of hate speech. Both the training set and the test set contain tweets related to hate speech against refugees, the Israel-Palestine conflict, and Anti-Greek discourse. The training set contains a total of 9,140 tweets. The distribution with respect to topics and labels is as follows: 5,924 tweets on Anti-Refugee sentiment (1447 hateful, 4477 non-hateful); 2,240 tweets on the Israel-Palestine conflict (880 hateful, 1,360 non-hateful), 976 tweets on Anti-Greek discourse (555 non-hateful, 421 hateful). 

- **Evaluation:** We will evaluate the hate speech detection performance of your best submitted model on the combined test data from all of the three topics. 

### Subtask B: Hate Speech Detection with Limited Data in Arabic

- **Objective:** To build a model for Arabic hate speech detection under data-constrained conditions.

- **Data:** A dataset of around 1000 Arabic tweets, particularly focusing on anti-refugee hate speech. This task is challenging with a smaller data set and high class imbalance.

- **Evaluation:** We will evaluate the model performance using test data, which includes tweets related to anti-refugee hate speech. 

## Dataset

Due to Twitter's Rules and Policies, tweet texts  cannot be shared publicly. To facilitate your participation in this shared task, we will distribute the necessary dataset via email. It's strictly prohibited to share or publish any data other than tweet IDs. Do not share or publish the dataset without obtaining permission first.

## Evaluation
Evaluation will be conducted on the Kaggle platform, allowing multiple, but limited number of submissions per team (you can make 3 submissions each day; after reaching this limit, participants will need to wait until the next day (UTC) to submit again). Rankings will be based on the best performance per team. The contest on Kaggle provides submission formats and further details. The evaluation metric for all subtasks will be the F1 score obtained on the test data. During the testing phase, two distinct leaderboards will be implemented. 

The initial leaderboard, constituting approximately 20% of the test data, is referred to as the public leaderboard and will be visible as feedback to the participants. In contrast, the private leaderboard, accounting for 80% of the test data, will remain concealed until after the testing phase and will determine the ultimate scores of the competition. 

In addition to the outcomes displayed on the Private Leaderboard, participants are required to provide their code along with a concise (150-250 words) model description. The submitted code must be error-free and capable of generating predictions identical to those submitted on the Kaggle platform to re-generate the final leaderboard score. If participants fail to provide error-free code that gives the given output, or their model description, their ranking and submissions will not be taken into consideration.

###  What to Submit
- **Full code:** You should upload your full code (containing pre-processing, training, and testing steps). Additionally, provide a README that explains how to execute the code for each task to ensure reproducible results.
- **Results:** You should submit a single csv file for each task, consisting of one line for each tweet; each line should contain a tweet ID and a corresponding label. Please use '1' to indicate the presence of hate speech and '0' to signify its absence. There must also be a header line "ID,Prediction". A sample submission file with correct format will be provided to the participants.
  
**Sample Submission File Format:**  
```
ID,Prediction
1,1
2,0
3,0
4,1
5,0
6,1
7,1
8,1
9,0
10,0
```

## Participation
Interested parties must fill out [the registration form](https://forms.gle/47eqrCuqMCe4KmxA7) and should join the corresponding Kaggle competitions:
- Subtask A: [TBA]
- Subtask B: [TBA]

### Award
There is an award prize for each task, to be distributed to top ranking submissions in each task, depending on their performances. The total amount for the full competition is 7000 euros (brut) to be distributed at the discretion of the evaluation committee according to the performance of the eligible submissions. 

## Timeline

* Registration Deadline: Jan 5, 2024
* Training Data Release (Subtask A): Dec 20, 2023
* Training Data Release (Subtask B): Dec 26, 2023
* Test Data Release: Jan 14, 2024
* Testing Phase: Jan 14-16, 2024
* Paper Submission Deadline: Jan 23, 2024
* Author Notification: Jan 29, 2024
* Final Paper Submission: Feb 2, 2024
* Workshop Dates: [To be Announced]

## Contact
For questions concerning the shared task, please contact gokceuludogan@gmail.com
