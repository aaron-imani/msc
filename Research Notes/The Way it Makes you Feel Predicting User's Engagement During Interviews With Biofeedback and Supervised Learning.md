# The Way it Makes you Feel Predicting User's Engagement During Intreviews With Biofeedback and Supervised Learning
## Paper Link

https://ieeexplore.ieee.org/document/9218155

## Research Questions

- What range of engagement do users report during an interview?
- To what extent can we predict users’ engagement using biofeedback measurements and supervised classifiers?

## Brief Summar

The paper aims to extend the body of knowledge in affective RE by studying users’ emotions during interviews. It has been focused on *engagement*—i.e., **the degree of positive or negative interest on a certain product-related aspect discussed in the interview**. They have performed a study with 31 participants taking part in a simulated interview during which they have captured participants’ biofeedback using an Empatica E4 wristband, and collect their self-assessed engagement. They compared different machine learning algorithms to predict users’ engagement based exclusively on features extracted from biofeedback signals.

They have used a dimensional representation of developers’ emotions. Specifically, we adopt the *Circumplex Model of Affect* by Russel, which represents emotions according to two continuous dimensions:
- valence (from pleasant to unpleasant)
- rousal (from activation to deactivation). 

In order to capture users’ biofeedback, they have used a noninvasive device that participants can comfortably wear during interviews called **Empatica E4** to collect electrodermal activity that correlates with the arousal dimension, blood volume pressure in which significant changes are observed in response to increase cognitive and mental load, and heart rate in which increases occur when the body needs a higher blood supply, for instance in presence of mental or physical stressors.

31 active Facebook users among the students of Kennesaw State University with an opportunistic sampling has been selected to attend an interview as the user interview questions dealt with this social network. According to the differences in biometrics due to physiological aspects, they have tried to have a pool of participants as varied as possible by including multiple ethnic groups and both female and male subjects.

Three main roles are involved in the experiment: *interviewer*, *user*, and *observer*. The interviewer leads the experiment by asking questions to the user, while the observer tracks the interview by annotating timestamps of each question, monitoring the output of the wristband, and annotating general observations on the interview and behaviour of the user. The experimental protocol consists of four phases:

1- Device calibration and emotion triggering: Using a set of emotion-triggering pictures, a short emotion elicitation task is runned to make paritcipants acquainted with the emotion self-report task, collect data to adjust the scores obtained during the self-assessment questionnaire, and to check the correct acquisition of the signal by letting the wristband record the raw signals for all biometric sensors under the experimenter scrutiny.

2- User’s interview: A trained interviewer conducts the interview with each user. The interview script consists of 38 questions concerning the Facebook platform. Questions are grouped into seven topics—i.e., usage habits, privacy, procedures, relationships, information, money, and ethics

3- Self-assessment questionnaire: For each question in the interview script (i.e., Qi), the interviewer asks the participant to report their involvement using two 10-point rating scale items: (qA(Qi)) How much did you feel involved with this topic? (1 = Not at all involved; 10 = Extremely involved); (qV (Qi)) How would you rate the quality of your involvement? (1 = Extremely negative; 10 = Extremely positive).

4- Wrap-up: The observer downloads and stores the wristband data as well as the questionnaires filled by the
participant. The wristband memory is then erased to allow further recording sessions.

After the interview, the collected signal data is used to elicit some signal features in a a binary classification task using machine learning. The classifiers are evaluated in a Hold-out setting. Thus, the the gold standard is splitted into train (70%) and test (30%) sets using the *stratified sampling* strategy.*Leave-one-out cross validation* is adpoted then to search for the optimal hyperparameters. Below, the results of the analysis is discussed and the RQs are answered.

- RQ1: We see that, overall, users tend to give high scores both for arousal and valence (both averages are above 7), indicating that the interview is generally perceived as positively engaging. Also, we see that the standard deviation is not particularly large, especially for valence which means that subjects tended to report scores around the average, and that apparently most of the interview triggered a similar level of engagement.

- RQ2: Yes, we can predict users’ engagement by combining biometric features into vectors and by training a Random Forest algorithm. We see that the Random Forest algorithm (rf) achieves the best performance across all the measures considered. The results indicate that the classifiers’ behavior is substantially better than the baseline classifier that always predicts the positive class.

## Findings

- Users’ interviews are activities that can trigger positive engagement in the involved users.
- Different levels of engagement are experienced depending on the topic of the question
- By combining biometric features into vectors and by training a Random Forest algorithm, it is possible to predict the engagement in a way that outperforms a majorityclass baseline.

## Suggested Future Work

* Be extended to large scale scenarios, for example for A/B testing, when low-cost devices will be available to acquire the considered measurements.
* Complement the analysis with the usage of other emotion-revealing signals considered in other studies, such as facial expressions captured through cameras, voice recording, and electroencephalographic (EEG) activity data.
* Apply the study protocol to requirements elicitation interviews for novel products to be developed.
* Investigate requirements analyst’s emotions in relation with users’ emotions during interviews, to explore the emotional dialogue that occurs between the two of them.
* Investigate and compare the emotional footprint of different softwarerelated tasks

## Relevance to my work

Considering the ATTACH project, we have a project with varietes of non-technical stakeholders. In such cases, uncertainty can affect elicitated software requirements. We can conduct a research to analyse the stakeholders’ biofeedback during requirements elicitation sessions to detect requirements on which some stakeholders doubt, so that  software engineers won't try implementing uncertain requirements.
