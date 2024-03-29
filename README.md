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

In addition to the outcomes displayed on the Private Leaderboard, participants are required to provide their code along with a concise (500 words) model description. The submitted code must be error-free and capable of generating predictions identical to those submitted on the Kaggle platform to re-generate the final leaderboard score. If participants fail to provide error-free code that gives the given output, or their model description, their ranking and submissions will not be taken into consideration.

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
- [Subtask A](https://www.kaggle.com/t/751541fe1dc943eaa415f7368fee6137)
- [Subtask B](https://www.kaggle.com/t/da35bee8c509493bb6239ef188db9ec7)

### Award
There is an award prize for each task, to be distributed to top ranking submissions in each task, depending on their performances. The total amount for the full competition is 7000 euros (brut) to be distributed at the discretion of the evaluation committee according to the performance of the eligible submissions. 

## Timeline

* Registration Deadline: Jan 5, 2024
* Training Data Release (Subtask A): Dec 23, 2023
* Training Data Release (Subtask B): Dec 26, 2023
* Test Data Release: Jan 14, 2024
* Testing Phase: Jan 14-16, 2024
* Paper Submission Deadline: Jan 25, 2024
* Author Notification: Jan 30, 2024
* Final Paper Submission: Feb 3, 2024
* Workshop Dates: Mar 21-22, 2024

## Paper Submission
Paper submission is not required for participation in the shared task. However, each participant is expected to provide a 500-word system description explaining their approach, any additional data used, and any other resources utilized (e.g., public code or pretrained networks).

In addition to system descriptions, short papers (https://aclrollingreview.org/cfp) will also be accepted to the shared task, but are not mandatory. Accepted papers will appear in the proceedings if written according to the guidelines of the ACL and may be presented in short-oral or poster format. At least one author must be registered to the workshop for publication.

Further details on submission requirements can be found at [https://emw.ku.edu.tr/case-2024/](https://emw.ku.edu.tr/case-2024/).

## Leaderboard Announcements

### Subtask A Leaderboard Results

1. **DetectiveReaders** with an F1 score of 0.69645 on the private leaderboard (sequestered test set).
   - **Team Members:** Fatima Zahra Qachfar, Bryan Tuck, Rakesh M. Verma
   - **Prize:** 1500€<sup>*</sup>

2. **ReBERT** with an F1 score of 0.68886 on the private leaderboard (sequestered test set).
   - **Team Members:** Egemen İşcan, Ahmet Emirhan Kolçak, Utku Uğur Yağcı
   - **Prize:**  1300€<sup>*</sup>

3. **VRLLab** with an F1 score of 0.66432 on the private leaderboard (sequestered test set).
   - **Team Members:** Onur Varol, Ali Najafi
   - **Prize:**  1100€<sup>*</sup>

### Subtask B Leaderboard Results

1. **ReBERT** with an F1 score of 0.68354 on the private leaderboard (sequestered test set).
   - **Team Members:** Egemen İşcan, Ahmet Emirhan Kolçak, Utku Uğur Yağcı
   - **Prize:**  1300€<sup>*</sup>

2. **Team Curie** with an F1 score of 0.65854 on the private leaderboard (sequestered test set).
   - **Team Members:** Işık Topçu, Ehsan Barkhordar
   - **Prize:**  1100€<sup>*</sup>

3. **Team Uriel** with an F1 score of 0.63636 on the private leaderboard (sequestered test set).
   - **Team Members:** Uriel Nguefack Yefou
   - **Prize:**  700€<sup>*</sup>

*The prizes provided are gross amounts.

Well done to all teams for their excellent work and contributions!

## Contact
Gökçe Uludoğan (gokceuludogan@gmail.com)

Somaiyeh Dehghan (somaiyeh.dehghan@sabanciuniv.edu)
