# :fire_extinguisher:YOLOv5를 이용한 소화기 감지 모델<br><sub>- Fire extinguisher detection model using YOLOv5</sub>

## :globe_with_meridians:프로젝트 개요 <sub>Overview of the Project</sub>

### :small_blue_diamond:배경 정보 소개 <sub>Opening Background Information</sub>

  - 화재 사고 발생 시 소화기를 빠르게 찾는 것은 초기 화재 진압의 핵심이다. 하지만 실제 상황에서 소화기를 빠르게 식별하는 것은 쉽지 않은 경우가 많다. 이를 해결하기 위해 머신러닝을 활용한 소화기 감지 기술을 사용하면 안전성과 효율성을 크게 높일 수 있다. 예를 들어, 로봇이 소화기를 찾고, 주변 사람을 해당 위치로 유도하는 등의 방법을 통해 화재를 빠르게 진압할 수 있다.<br>
      <sub>In the event of a fire accident, quickly finding a fire extinguisher is the key to initial fire suppression. However, in real situations, it is often not easy to quickly identify a fire extinguisher. To solve this, fire extinguisher detection technology using machine learning can greatly improve safety and efficiency. For example, a robot can quickly extinguish a fire by finding a fire extinguisher and guiding nearby people to that location.</sub>

### :small_blue_diamond:프로젝트의 전반적인 설명 <sub>General Description of the Current Project</sub>

  - 이 프로젝트는 소화기를 감지하는 딥러닝 모델을 개발하는 것을 목표로 한다. YOLOv5와 같은 실시간 객체 탐지 모델을 활용하여 다양한 환경에서 소화기를 정확히 탐지하고, 이를 기반으로 알림 시스템과 통합하여 화재 발생 시 신속하게 대응할 수 있는 솔루션을 제안한다. 또한, 소화기 감지 기능을 탑재한 로봇이 가정 내 화재 발생 시 소화기 위치를 파악하고 사람에게 알려주는 시스템을 제시하여 화재 초기에 신속한 대응이 가능하도록 한다.<br>
      <sub>This project aims to develop a deep learning model that detects fire extinguishers. Using real-time object detection models such as YOLOv5, we propose a solution that accurately detects fire extinguishers in various environments and integrates this with a notification system to quickly respond to fires. In addition, we propose a system in which a robot equipped with a fire extinguisher detection function identifies the location of a fire extinguisher and notifies people when a fire occurs in the home, enabling a quick response in the early stages of a fire.</sub>

### :small_blue_diamond:제안하고 싶은 프로젝트의 강점 <sub>Proposed Idea for Enhancements to the Project</sub>

  1. **실시간 감지**: YOLOv5를 활용해 소화기를 실시간으로 감지하여 즉각적인 대응이 가능하다.<br>
      <sub>**Real-time detection**: YOLOv5 can be used to detect fire extinguishers in real time, enabling immediate response.</sub>


  2. **여러 각도에서의 촬영**: 초기 모델 학습 시, 비슷한 구도에서만 촬영된 영상으로는 정확도가 낮았으며, 다양한 각도에서 촬영한 데이터를 활용하여 정확도를 크게 향상시켰다.<br>
      <sub>**Shooting from multiple angles**: During initial model training, the accuracy was low with images shot only from similar angles, and the accuracy was greatly improved by utilizing data shot from various angles.</sub>


  3. **화재 진압 기능이 없는 로봇에도 적용 가능**: 소화기 감지 모델을 화재 진압 기능이 없는 가정용 로봇에 탑재하여, 화재 발생 시 소화기 위치를 빠르게 찾고 주변 사람에게 알려주거나 해당 위치로 유도할 수 있다.<br>
      <sub>**Can also be applied to robots without fire suppression functions**: By installing the fire extinguisher detection model on a home robot without a fire suppression function, the location of the fire extinguisher can be quickly found in the event of a fire, and the location can be notified to people or guided to the location.</sub>


### :small_blue_diamond:프로젝트의 가치와 중요성 <sub>Value and Significance of this Project</sub>

  - 소화기 탐지 시스템은 화재 안전 관리에서 중요한 역할을 한다. 이 프로젝트는 화재 발생 시 초기 대응 시간을 줄이고, 화재 피해를 최소화할 수 있는 잠재력을 제공한다. 공공시설, 산업 현장 등 다양한 공간에서 활용 가능하며, 스마트 안전 시스템의 필수 요소로 자리잡을 수 있다. 특히 가정용 로봇에 소화기 탐지 기능을 탑재함으로써, 화재 발생 초기 대응에 대한 안전성을 더욱 강화할 수 있다.<br>
      <sub>The fire extinguisher detection system plays an important role in fire safety management. This project offers the potential to reduce the initial response time and minimize fire damage in the event of a fire. It can be used in various spaces such as public facilities and industrial sites, and can become an essential element of a smart safety system. In particular, by installing a fire extinguisher detection function in a home robot, the safety of the initial response to a fire can be further strengthened.</sub>

### :small_blue_diamond:직면하고 있는 한계 <sub>Current Limitations</sub>

  1. 다양한 환경에서 소화기를 탐지하는 데 있어 배경과 소화기의 색상, 형태가 유사한 경우 혼동이 발생할 수 있다.<br>
        <sub>When detecting fire extinguishers in various environments, confusion may occur when the background and the fire extinguisher have similar colors and shapes. 2. It is necessary to set a balance between real-time detection speed and model accuracy. </sub>
  
  2. 실시간 감지 속도와 모델의 정확성 간 밸런스 설정이 필요하다.<br>
        <sub>A balance between real-time detection speed and model accuracy is needed.</sub>

### :small_blue_diamond:문헌 고찰 <sub>Literature Review</sub>

  - 소화기 탐지를 위한 객체 탐지 기술과 관련된 기존 연구를 조사하였다. 특히, YOLO 시리즈의 성능과 데이터셋 구성 방식, 그리고 다양한 환경에서의 모델 성능을 향상시키는 방법에 대한 연구를 참고하여 프로젝트 설계를 진행하였다.<br>
      <sub>We investigated previous research on object detection techniques for fire extinguisher detection. In particular, we designed the project by referring to research on the performance of the YOLO series, the dataset composition method, and how to improve model performance in various environments.</sub>

---

## :memo:학습 과정 <sub>Learning Process</sub>

<sub>[결과물 바로가기 <sub>Go to RESULT</sub>](runs/detect/jetsonVideo.mp4)</sub><br>


### :small_orange_diamond:영상 취득 방법 <sub>Image Acquisition Method</sub>

  - **실제 환경 데이터 수집**: 다양한 건물 내부에서 소화기를 촬영하여 실제 데이터를 확보하였다.<br>
      <sub>**Real-world data collection**: Real-world data was obtained by filming fire extinguishers inside various buildings.</sub>

    <sub>[원본 영상 바로가기 <sub>Go to original video</sub>](train/videos/20241115_175106.mp4)</sub><br>
     ![실제 촬영 영상](forReadMeFile/sourceVideo.gif)


### :small_orange_diamond:학습 데이터 추출과 학습 어노테이션 <sub>Learning Data Extraction and Learning Annotation</sub>

  - 촬영된 영상을 프레임 단위 이미지로 만들고 어노테이션을 하기 위해서 Video/Image Labeling and Annotation Tool로 잘 알려진 [DarkLabel](DarkLabel2.4)을 사용했다.<br>
      <sub>To create frame-by-frame images or annotate the captured video, [DarkLabel](DarkLabel2.4), well known as a Video/Image Labeling and Annotation Tool, was used.</sub>

  1. **[DarkLabel.exe](DarkLabel2.4/DarkLabel.exe) 설치한다.**<br>
     <sub>**Install [DarkLabel.exe](DarkLabel2.4/DarkLabel.exe).**</sub>

  2. **[darklabel.yml](DarkLabel2.4/darklabel.yml) 파일을 수정한다.**<br>
     <sub>**Modify the file [darklabel.yml](DarkLabel2.4/darklabel.yml)**</sub>

      2-1. 15번 줄에 `"my_classes2: ["fireExt"]"`을 추가한다.<br>
      <sub>Add `"my_classes2: ["fireExt"]"` on line 15.</sub>

      2-2. 66번 줄을 `classes_set: "my_classes2"`으로 수정한다.<br>
      <sub>Change line 66 to `classes_set: "my_classes2"`.</sub>

  3. **DarkLabel 프로그램을 실행한다.**<br>
     <sub>**Run the DarkLabel program.**</sub>

  4. **학습에 사용할 영상을 `Open Video`을 통해 가져온다.**<br>
     <sub>**Load the video for training via `Open Video`.**</sub>
     
     ![DarkLebel_Screenshots](forReadMeFile/DarkLabel_Screenshots.png)

  5. **위와 같이 설정하고 학습에 필요한 객체를 Box로 표시한다.**<br>
     <sub>**Set up as shown above and mark the objects required for training using boxes.**</sub>

      5-1. `shift + right-click`: 박스 삭제 <sub>Delete box</sub><br>
      5-2. `shift + left-click`: 박스 이동 <sub>Move box</sub><br>
      5-3. `space bar`: 다음 프레임으로 이동 <sub>Move to the next frame</sub>

  6. **모든 프레임에 라벨링을 한 후, 각 데이터 파일을 다운 받는다.**<br>
     <sub>**After labeling all frames, download each data file.**</sub>
     
      6-1. `as Images..`: 각 프레임의 [이미지](train/images) 저장 <sub>Save each frame as an [image](train/images)</sub><br>
      6-2. `GT Save As..`: 각 프레임의 [라벨 값](train/labels) 저장 <sub>Save the [label values](train/labels) for each frame(train/labels)</sub>


        <sub>[원본 영상 바로가기 <sub>Go to original video</sub>](train/videos/20241115_175106_gt.avi)</sub><br>
     ![labelVideo](forReadMeFile/labelVideo.gif)


### :small_orange_diamond:Nvidia Jetson Nano 학습 과정 <sub>Nvidia Jetson Nano Training Process</sub>

  - 구글 코랩을 이용하여 학습하였다.<br>
      <sub>The training was conducted using Google Colab.</sub>
    
  - 상세 과정은 [여기](yolov5_ai_specialist.ipynb)에서 확인할 수 있다.<br>
      <sub>Detailed steps can be found [here](yolov5_ai_specialist.ipynb).</sub>

  - 학습에 필요한 라이브러리<br>
      <sub>Libraries required for learning</sub><br>
     ```python
     import torch
     import os
     from IPython.display import Image, clear_output  # to display images
     ```

  - 학습 스크립트<br>
      <sub>Script for learning</sub><br>
     ```python
     !python train.py  --img 512 --batch 16 --epochs 300 --data /content/drive/MyDrive/yolov5/data.yaml --weights yolov5n.pt --cache
     ```

     - `--img 512`: 입력 이미지의 크기를  512*512로 설정한다.<br>
     <sub>Set the size of the input image to 640x640.</sub>
     
     - `--batch 16`: 배치 크기를 설정한다. 한 번에 처리되는 이미지의 수를 나타낸다.<br>
     <sub>Sets the batch size. This indicates the number of images to be processed at one time.</sub>
     
     - `--epochs 300`: 학습할 총 에폭(epoch) 수를 설정합니다.<br>
     <sub>Sets the total number of epochs to learn.</sub>
     
     - `--data /content/drive/MyDrive/yolov5/data.yaml`: 데이터셋 및 모델 구성에 대한 설정이 담긴 [YAML](data.yaml) 파일의 경로를 지정한다.<br>
     <sub>Specifies the path to the [YAML](data.yaml) file containing the configuration settings for the YOLOv5 model.</sub>
     
     - `--weights yolov5n.pt`: 미리 훈련된 가중치 파일의 경로를 지정한다. 여기서는 [yolov5n.pt](yolov5n.pt) 파일을 사용하고 있다.<br>
     <sub>Specifies the path to the pre-trained weights file. Here, we are using the [yolov5n.pt](yolov5n.pt) file.</sub>


### :small_orange_diamond:Nvidia Jetson Nano 학습 결과 <sub>Nvidia Jetson Nano Training Result</sub>

  - 학습 결과는 `/content/drive/MyDrive/yolov5/runs/train`에 저장된다.<br>
      <sub>Training results are stored in `/content/drive/MyDrive/yolov5/runs/train`.</sub>

  - 리포지토리 내에서는 [여기](runs/train)에서 확인할 수 있다.<br>
      <sub>In the repository, the results can be checked [here](runs/train).</sub>

| **F1 Curve** | **PR Curve** |
|--------------|--------------|
| ![F1 Curve](runs/train/exp2/F1_curve.png) | ![PR Curve](runs/train/exp2/PR_curve.png) |

| **P Curve**  | **R Curve**  |
|--------------|--------------|
| ![P Curve](runs/train/exp2/P_curve.png)   | ![R Curve](runs/train/exp2/R_curve.png)   |

| **Results**  |
|--------------|
| ![Results](runs/train/exp2/results.png)   |


### :small_orange_diamond:Nvidia Jetson Nano 학습 결과 검증 영상 <sub>Nvidia Jetson Nano Training Results Verification Video</sub>
  - 비교적 어두운 곳과 밝은 곳, 정면과 측면 모두 정확히 감지하는 것을 알 수 있다.<br>
      <sub>It can be seen that detection is accurate in relatively dark and bright places, both front-facing and from the side.</sub>


     <sub>[원본 영상 바로가기 <sub>Go to original video</sub>](runs/detect/exp6/20241115_112352.mp4)</sub><br>
     ![resultVideo](forReadMeFile/resultVideo.gif)

<sub>[결과물 바로가기 <sub>Go to RESULT</sub>](runs/detect/jetsonVideo.mp4)</sub><br>
