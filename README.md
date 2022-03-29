# Don’t Sleep Driver
### What is Don’t Sleep Driver?
Every year, drowsy driving causes numerous traffic accidents and many people are injured or killed. In Korea, 70% of deaths in highway traffic accidents are due to drowsiness or neglect.
The death rate from drowsy driving is much higher than drunk driving, but awareness of the risks is very low. Drivers who drive alone for long periods of time are vulnerable to drowsy driving.
So, to solve this problem, we created an app to prevent drowsy driving called Dont Sleep Driver.
## Feature
Users can sign in with their email and password and can easily sign up and sign in with OAuth2.0 technology.
When the user starts driving and presses the start button of the app, it recognizes faces through the camera and determines whether or not they are asleep.
If the user is drowsy while driving, a warning alarm will sound, as well as an alarm for stretching and ventilation every 30 minutes and 2 hours.
You can end driving and inquire about your driving record, gps information and sleep level in the record tab.
## Demo Video
[![DontSleepDriver](https://user-images.githubusercontent.com/28949213/160598053-71f9ecef-3304-46b9-bb6c-170dade75c15.png)](https://youtu.be/OeRTsWqkZ1Y)
## Repositories
- [Android](https://github.com/gdsc-seoultech/DontSleepDriver_Android)
- [ML](https://github.com/gdsc-seoultech/DontSleepDriver_ML)
- [BackEnd](https://github.com/gdsc-seoultech/DontSleepDriver_Back)
## 👨‍: Team Member
<table algin=“center”>
   <tr>
      <td colspan=“2" align=“center”><strong>Back-End</strong></td>
      <td colspan=“1" align=“center”><strong>Android</strong></td>
      <td colspan=“1" align=“center”><strong>ML</strong></td>
   </tr>
  <tr>
     <td align=“center”>
        <a href=“https://github.com/InHyeok-J”><img src=“https://avatars.githubusercontent.com/u/28949213?v=4” width=“150px” alt=“조인혁“/><br /><sub><b>조인혁</b></sub></a>
     </td>
    <td align=“center”>
    <a href=“https://github.com/ehrwk”><img src=“https://avatars.githubusercontent.com/u/81352045?v=4” width=“150px;” alt=“윤희서“/><br /><sub><b>윤희서</b></sub></a><br />
    </td>
     <td align=“center”>
        <a href=“https://github.com/comye1”><img src=“https://avatars.githubusercontent.com/u/50735594?v=4” width=“150px” alt=“김예원“/><br /><sub><b>김예원</b></sub></a>
     </td>
     <td align=“center”>
        <a href=“https://github.com/keonju2”><img src=“https://avatars.githubusercontent.com/u/54880474?v=4” width=“150px” alt=“나건주“/><br /><sub><b>나건주</b></sub></a>
  <tr>
</table>


## Build the demo using Android Studio

### Prerequisites

*   If you don't have already, install
    **[Android Studio](https://developer.android.com/studio/index.html)**,
    following the instructions on the website.

*   You need an Android device and Android development environment with minimum
    API 21.

*   Android Studio 3.2 or later.

### Building

*   Open Android Studio, and from the Welcome screen, select Open an existing
    Android Studio project.

*   From the Open File or Project window that appears, navigate to and select
    the tensorflow-lite/examples/object_detection/android directory from
    wherever you cloned the TensorFlow Lite sample GitHub repo. Click OK.

*   If it asks you to do a Gradle Sync, click OK.

*   You may also need to install various platforms and tools, if you get errors
    like "Failed to find target with hash string 'android-21'" and similar.
    Click the `Run` button (the green arrow) or select `Run > Run 'android'`
    from the top menu. You may need to rebuild the project using `Build >
    Rebuild` Project.

*   If it asks you to use Instant Run, click Proceed Without Instant Run.

*   Also, you need to have an Android device plugged in with developer options
    enabled at this point. See
    **[here](https://developer.android.com/studio/run/device)** for more details
    on setting up developer devices.

### Models

*   Yolov5s
*   Input data : [1 , 320, 320, 3]

### Test Python  
  
```python
!git clone https://github.com/gdsc-seoultech/DontSleepDriver_ML/detect  # clone repo  
!pip install -r requirements.txt # install dependencies  

!python detect.py --source {Image Path} --weights {best.pt Path} --name exp  
```
