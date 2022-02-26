# DeepFake Workshop cum Hackathon

Hosted by DIC, UIET, Panjab University, Chandigarh

Register [here](https://dare2compete.com/p/idfd-challenge-265681) to participate in IDFD. Only registered participants will be able to see shared data.
Last date to register: 06-March-2022
Tutorial Session on 05-March-2022 @ https://meet.google.com/wwh-tcag-myt

<hr>

<p align="center">
  <a href="#Overview">About</a> &#xa0; | &#xa0; 
  <a href="#Competition_Stages">Competition Stages</a> &#xa0; | &#xa0;
  <a href="#Competition_Rules">Competition Rules</a> &#xa0; | &#xa0;
  <a href="#References" >References</a>
</p>

<br>

## Overview
Deepfake refers to facially manipulated images and vidoes of people. The technology is growing fast and is a greatest threat to the dignity of common man. With advancement in AI technology, deepfake creation techniques are also improving. Since this creation and detection is a two-party game which is never going to end, we are organizing a competition to provide a benchmark this game between user-friendly generation techniques and most efficient detection techniques for the same. The outcome of this competition would be a set of Indian deepfakes which will help the research community and a detection technique for the generated dataset.

## Competition_Stages

### First round: Deepfake Creation:
In this phase, a team is needed to capture images and generate fake images from them using the given code. 
1. Collect samples of real images and 3-second videos of different subjects. Each image and video must exhibit face area of single person, positioned at centre position. No two teams should have same set of images/videos or images/videos of same subject. For each subject, maximum 50 images and 50 videos are allowed. 
2. Generate deepfake videos and images through below given methods: 
- **FOM**: First Order Motion Model [1] ([Here](https://colab.research.google.com/drive/1cniN2Tm9yqmZE6XfDtMzLVSouY1e7S7e?usp=sharing) is a colab file to generate data). Sample dataset is also provided with the code. For detailed information refer to original github: https://github.com/AliaksandrSiarohin/first-order-model

<p align="center">
<img src = "https://user-images.githubusercontent.com/54838730/147690041-869fd427-2826-4c6b-9d45-1717c6fde1db.gif" width="200" height="200"/> <img src= "https://user-images.githubusercontent.com/54838730/147691508-3937a775-e4c9-4b41-b691-09ba404b3282.png" width="350" height="200"/> <img src="https://user-images.githubusercontent.com/54838730/147690060-ca5c4822-d2af-4e11-a844-b0ce933360d9.gif" width="200" height="200"/>
</p>
   
 - **FaceApp**:Install Mobile Application, FaceApp [2] and use feature FaceSwap there. Input different pairs of images as source and target image.

<p align="center">
  <img src="https://user-images.githubusercontent.com/54838730/147633573-414c347f-aca4-4335-97a9-c66e75226795.png" />
</p>

At Level 1, teams are evaluated on the basis of diversity and quantity of subjects captured and deepfaked.

### Second round: Deepfake Detection:
In this phase, selected teams from first round would have to train existing deep learning models on data generated in first round. A sample kernel is provided [here](https://colab.research.google.com/drive/1gvWIA3YrpmQlOmCSDabMVcScM_nMAQWz?usp=sharing). A team can also create a new detection mechanism. Detailed steps are given as follows:
1. From each video generated in FOM and originally captured ones, extract maximum of 5 frames.
2. Generate two sets 
   - **Dataset 1:** FOM + Real image dataset
   - **Dataset 2:** FaceApp + Real image dataset 
4. Try every model with both datasets separately. Select the model and respective parameters that work well for both datasets separately.  
5. Share the best trained models with final notebooks that contain results. We will test the trained model on private test set. Winner is selected based on the results on private test set.

## Competition_Rules:
1. Maximum 4 members can join in a team. 
2. This challenge exhibit two levels; performance of team is evaluated after each level and elimination is done accordingly. Top 50% teams from Level-2 would be admitted to Level-2. 
3. Participation certificate will be provided.
4. Atleast one team member should have knowledge of python language.
5. In round 1,
    - No two teams can submit same set of images/videos.
    - No two teams can submit images/videos of same person.


## References
1. Siarohin, A., Lathuilière, S., Tulyakov, S., Ricci, E., & Sebe, N. (2019). First order motion model for image animation. Advances in Neural Information Processing Systems, 32, 7137-7147.
2. https://www.faceapp.com/
