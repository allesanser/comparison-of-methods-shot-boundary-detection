# comparison-of-methods-shot-boundary-detection

Here i'm going to compare sota models of shot boundary detection.   

First of all, a little about the structure of a video sequence. Video consists of frames. In editing, frames are cut into groups which are rearranged according to the director's ideas and glued back together. The sequence of frames from one montage to the next is called a shot. Shots are grouped together by meaning, they are called scenes. A scene is characterised by the unity of place, time and characters.  

There are two approaches for finding scene boundaries:  
1) Take the whole video and search for scene boundaries  
2) First, divide the video into shots and then merge them into scenes   


Most shot boundary detection algorithms work in 2 steps:
* Calculating the value of the frame difference metric or metrics
* Setting the threshold for frame classification. Also at this stage, machine learning is often
used for automatic classification.
* An additional step can be filtering frames for false positive detections.

![image](https://user-images.githubusercontent.com/52531828/175067025-01a56a06-79df-453c-a5a9-4255c479fbaf.png)

# Models
## TransNet V2: Shot Boundary Detection Neural Network

https://github.com/soCzech/TransNetV2  
 <a href="https://colab.research.google.com/drive/1Zaip4cc1FzplanXoviUxN5Zbu4CaoiX5?authuser=1#scrollTo=LHPLHWirC4mQ"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="google colab logo"></a>  
   The model performs quite well. The picture shows all the frames in the video, and you can see blue bars on the boundaries of the scenes - the model's prediction that a scene has ended/began. Video processing speed - extremely fast.  
 ![1a512101-1389-4a09-9a79-552ae50fed8a](https://user-images.githubusercontent.com/52531828/175001668-7e23894e-c16b-4d6f-8e3e-41d803d444f0.png)  
 Handles complex video well, too. (https://www.youtube.com/watch?v=rT22nYLaVbo&t=315s&ab_channel=DarryVideoEdit). False transitions are marked in red and true transitions in green. 
 ![Iron mp4 vis](https://user-images.githubusercontent.com/52531828/175267863-e9bf5992-fe52-43d8-89fb-a509f9c0525c.png)

 This model is used in Googl's mediapipe. 
 
 ## SceneSeg
 https://github.com/AnyiRao/SceneSeg 
 
 <a href="https://colab.research.google.com/drive/1dH95TWU47wKXSaoV_IHWktmjYy8Su7BR?authuser=1#scrollTo=fpqcPnyR8vRg"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="google colab logo"></a>  
 On a simple video, it gave out shots like the previous model.  
Performs worse with large videos than the previous model. Processing speed ~ 160 fps
 
 # TODO  
 

https://github.com/Tangshitao/ClipShots_basline - ???????? ???? ??????????????????????  
https://github.com/melgharib/DSBD                                                                   - ???? matlab
 
 
 https://github.com/johmathe/Shotdetect -                                                              ????????????????????, ?????????? ?????????? ???? ???????????????????? ????????????????  
 https://github.com/yahoo/hecate -                                                                     ???????????????????? ???? C++  
 https://arxiv.org/pdf/2109.01057.pdf                                                                  ???????????? ???? ?????? ????????????, ?????????? ??????  
 https://github.com/hoffsupes/Shot-boundary-detection-using-SVM-s-Aritificial-Neural-Networks-and-kNN


 
 

