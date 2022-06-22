# comparison-of-methods-shot-boundary-detection

Here i'm going to compare sota models of shot boundary detection.   

First of all, a little about the structure of a video sequence. Video consists of frames. In editing, frames are cut into groups which are rearranged according to the director's ideas and glued back together. The sequence of frames from one montage to the next is called a shot. Shots are grouped together by meaning, they are called scenes. A scene is characterised by the unity of place, time and characters.  

There are two approaches for finding scene boundaries:  
1) Take the whole video and search for scene boundaries  
2) First, divide the video into shots and then merge them into scenes  


# Models
## TransNet V2: Shot Boundary Detection Neural Network

https://github.com/soCzech/TransNetV2  
 <a href="https://colab.research.google.com/drive/1Zaip4cc1FzplanXoviUxN5Zbu4CaoiX5?authuser=1#scrollTo=LHPLHWirC4mQ"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="google colab logo"></a>  
   The model performs quite well. The picture shows all the frames in the video, and you can see blue bars on the boundaries of the scenes - the model's prediction that a scene has ended/began. Video processing speed - extremely fast.  
 ![1a512101-1389-4a09-9a79-552ae50fed8a](https://user-images.githubusercontent.com/52531828/175001668-7e23894e-c16b-4d6f-8e3e-41d803d444f0.png)
 
 
 
 # TODO  
 
 https://habr.com/ru/company/ivi/blog/497428/                                                          иви  
 https://habr.com/ru/company/ivi/blog/497428/ -                                                        статья про объединение шотов в сцены    
 https://github.com/johmathe/Shotdetect -                                                              приложение, вроде чисто на алгоритмах работает  
 https://github.com/Tangshitao/ClipShots_basline -                                                     проверить  
 https://github.com/yahoo/hecate -                                                                     библиотека на C++  
 https://github.com/hoffsupes/Shot-boundary-detection-using-SVM-s-Aritificial-Neural-Networks-and-kNN  
 https://github.com/StanLei52/GEBD                                                                      Просто бенчмарк

 
 

