# Real-time Mahjong Object Detection Model 
Just for backup. May have some file miss.
This project is just for fun. Not any official project in company or school.  
Train Dataset and final trained weights are not provided in this repo.  
Android project and its app are lost. The android project is referred to Tensorflow Lite Offcial object detection project. Just for testing the performance on mobile device.  

## Background
In Chinese New Year, people love playing Mahjong(麻雀) with their friends or relations. In Hong Kong Mahjong, players need to get at least 3 points to meet the win requirement. Some Points Calculator applications in Google Play exist and depend on manual input players’ tiles to calculate the points.

It is amazing to imagine a fast and convenient way – the user can take a photo and get the points number directly. This project aims to train a real-time Mahjong object detection model to solve the manual tile input problem.


## Detail that may be helpful 
In this project, Yolov3, Yolo-tiny v4 model is trained using Darknet.
|-------------|Content|
| ------------- | ------------- |
| Train Dataset  | 183 photos  |
| Test Dataset  | 13 photos  |
| Trained Model size(Yolov3)  | 274MB |
| Trained Model size(Yolo-tiny v4)  | 35MB |

## Result  
Yolov3 vs Yolo-tinyv4
Yolov3 model size is too large(274MB). I can't believe a normal point calculator application has more than 200MB in size. Also, the mobile device will be very lag when running this model. But We can't deny that the accuracy is quite good.
Yolo-tinyv4 has a lesser size. And Having good performance in mobile devices. But its accuracy is not high. It always has miss detection. 

In colab  
<img src="https://user-images.githubusercontent.com/71573064/160240525-fb2772d0-5540-4079-908a-ecba83deece1.jpg" width="400"/>
  
In real-time Android device  
<img src="https://user-images.githubusercontent.com/71573064/160240535-1d414eaf-38e4-42c6-8d0c-1700236bb08a.jpg" width="400"/>

## File  
cudnn-10.0-linux-x64-v7.5.0.56.tgz  
https://developer.nvidia.com/compute/machine-learning/cudnn/secure/v7.5.0.56/prod/10.0_20190219/cudnn-10.0-linux-x64-v7.5.0.56.tgz

## Reference  
Export from chrome bookmarks 
<DT>
        <DL><p>
            <DT><A HREF="https://medium.com/@matus.tanon/custom-object-detection-using-tensorflow-in-google-colab-e4d6e1a17f18" ADD_DATE="1630498725">Custom Object Detection Using Tensorflow in Google Colab | by Matus Tanonwong | Medium</A>
            <DT><A HREF="https://towardsdatascience.com/detailed-tutorial-build-your-custom-real-time-object-detector-5ade1017fd2d" ADD_DATE="1630498725">Step by Step: Build Your Custom Real-Time Object Detector | by Alaa Sinjab | Towards Data Science</A>
            <DT><A HREF="https://blog.csdn.net/m0_37750065/article/details/104824745" ADD_DATE="1630498725">Google colab 阻止自动掉线_chadqiu的博客-CSDN博客</A>
            <DT><A HREF="https://github.com/chihimng/COMP4901J_Project" ADD_DATE="1630498725">GitHub - chihimng/COMP4901J_Project: Mahjong Tile Image Classification with Denoising CAE and CNN</A>
            <DT><A HREF="https://github.com/jerryxgh/Workspaces/blob/master/c%26c%2B%2B/%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B8%8E%E7%AE%97%E6%B3%95%E5%88%86%E6%9E%90/%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B8%8E%E7%AE%97%E6%B3%95%E5%88%86%E6%9E%90%E6%BA%90%E4%BB%A3%E7%A0%81%E4%B8%8E%E7%AD%94%E6%A1%88/%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B8%8E%E7%AE%97%E6%B3%95%E5%88%86%E6%9E%90%E7%AD%94%E6%A1%88/ch01.pdf" ADD_DATE="1630498725">Workspaces/ch01.pdf at master · jerryxgh/Workspaces</A>
            <DT><A HREF="https://towardsdatascience.com/detailed-tutorial-build-your-custom-real-time-object-detector-5ade1017fd2d#b948" ADD_DATE="1630498780">Step by Step: Build Your Custom Real-Time Object Detector | by Alaa Sinjab | Towards Data Science</A>
            <DT><A HREF="https://medium.com/@galaxian.cube/how-to-train-a-sylvanian-families-detector-using-yolov3-and-darknet-on-google-colab-f1cb983f1dac" ADD_DATE="1630498780">How to train a Sylvanian Families detector using YOLOv3 and Darknet on Google Colab | by Galaxian Cube | Medium</A>
            <DT><A HREF="https://blog.csdn.net/u010122972/article/details/77380785" ADD_DATE="1630498780">yolo模型移植到android手机端_搬砖笔记-CSDN博客</A>
            <DT><A HREF="https://github.com/natanielruiz/android-yolo" ADD_DATE="1630498780">natanielruiz/android-yolo: Real-time object detection on Android using the YOLO network with TensorFlow</A>
            <DT><A HREF="https://chtseng.wordpress.com/2018/09/01/%E5%BB%BA%E7%AB%8B%E8%87%AA%E5%B7%B1%E7%9A%84yolo%E8%BE%A8%E8%AD%98%E6%A8%A1%E5%9E%8B-%E4%BB%A5%E6%9F%91%E6%A9%98%E8%BE%A8%E8%AD%98%E7%82%BA%E4%BE%8B/" ADD_DATE="1630498780">建立自己的YOLO辨識模型 – 以柑橘辨識為例 – CH.Tseng</A>
            <DT><A HREF="https://gist.github.com/Amir22010/a99f18ca19112bc7db0872a36a03a1ec" ADD_DATE="1630498780">convert pascal voc dataset to yolo format</A>
            <DT><A HREF="https://github.com/pjreddie/darknet/issues/363" ADD_DATE="1630498780">Weight Model size reduction / optimization · Issue #363 · pjreddie/darknet</A>
            <DT><A HREF="https://chtseng.wordpress.com/2020/09/27/%E8%A6%BA%E5%BE%97yolo-tiny%E4%B8%8D%E5%A4%A0%E5%BF%AB%E5%97%8E%EF%BC%9F%E8%A9%A6%E8%A9%A6yolo-fastest/" ADD_DATE="1630498780">覺得YOLO-Tiny不夠快嗎？試試YOLO-Fastest – CH.Tseng</A>
            <DT><A HREF="https://zhuanlan.zhihu.com/p/33822125" ADD_DATE="1630498780">Darknet yolo 在 android studio上的移植和实现 - 知乎</A>
        </DL><p>
