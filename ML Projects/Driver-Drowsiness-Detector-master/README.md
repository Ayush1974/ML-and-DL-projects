
**Driver Drowsiness Detection**
Tweet: [https://twitter.com/intent/tweet?text=Check%20out%20Driver%20Drowsiness%20Detection%20project%20on%20Github%20&url=https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/&hashtags=python,drowsiness-detector,opencv,computer-vision,machine-learning,deep-learning](https://twitter.com/intent/tweet?text=Check%20out%20Driver%20Drowsiness%20Detection%20project%20on%20Github%20&url=https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/&hashtags=python,drowsiness-detector,opencv,computer-vision,machine-learning,deep-learning)  GitHub stars: [https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/stargazers](https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/stargazers)  GitHub forks: [https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/network](https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/network)

This program is designed to detect drowsiness in real-time. It works by monitoring eye closure and triggering an alarm if drowsiness is detected beyond a certain threshold.

**Functionality**

The program analyzes webcam footage to detect a person's face and eyes. It then calculates the Eye Aspect Ratio (EAR), a metric that indicates eye closure. If the EAR falls below a specific value for a sustained period, the program raises an alarm to alert the driver.

**Files**

The program consists of three core Python scripts:

* **face_and_eye_detector_single_image.py:** Detects faces and eyes within a single image.

  **Demo:**

  | Test Image | Result Image |
  |---|---|
  | Test Image: [https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/blob/master/images/test.jpeg](https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/blob/master/images/test.jpeg) | Result Image: [https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/blob/master/images/result_face_detector_single_image.png](https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/blob/master/images/result_face_detector_single_image.png) |

* **face_and_eye_detector_webcam_video.py:** Detects faces and eyes in a live webcam feed.

  Webcam Face and Eye Detection: [https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/blob/master/images/webcam_face_eye_detect.jpeg](https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/blob/master/images/webcam_face_eye_detect.jpeg)

* **drowsiness_detect.py:** Analyzes webcam video to detect drowsiness based on Eye Aspect Ratio.

  **Demo:**

  Drowsiness Detection Demo: [https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/blob/master/images/drowsiness_detector_demo.gif](https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/blob/master/images/drowsiness_detector_demo.gif)

**Requirements**

**Important:**

* Download `shape_predictor_68_face_landmarks.dat.bz2` from Shape Predictor 68 features: [http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2).
* Extract the file in the project folder using the following command:

```bash
bzip2 -dk shape_predictor_68_face_landmarks.dat.bz2
```

* The following Python libraries are required:

  ```bash
  numpy==1.15.2
  dlib==19.16.0
  pygame==1.9.4
  imutils==0.5.1
  opencv_python==3.4.3.18
  scipy==1.1.0
  ```

  You can install them using the following command:

  ```bash
  pip install -r requirements.txt
  ```

**Usage**

**Detect Face and Eyes in a Single Image**

1. Place the image you want to analyze in the `images` folder with the name `test.jpeg`.
2. Alternatively, modify the file path in `Line: 14` of `face_and_eye_detector_single_image.py` to point to your desired image.
3. Run the script using the following command:

   ```bash
   python face_and_eye_detector_single_image.py
   ```

**Detect Face and Eyes in a Webcam Feed**

Run the script using the following command:

```bash
python face_and_eye_detector_webcam_video.py
```

**Drowsiness Detection**
made with ❤️ by Ayush1974