## <pre>                              IT314 - Software Engineering </pre> 
### Lab 5 : Static Analysis Tool
### Name : Chintankumar Suthar
### ID: 202001242

---
## Static Analysis
- Static analysis is a method of examining the source code of a software program without
executing it. Static analysis can help detect errors, bugs, vulnerabilities, and other quality issues
in the code. Static analysis tools can perform various tasks such as checking syntax, style,
logic, data flow, control flow, and security. Static analysis can improve the reliability,
performance, and maintainability of software by identifying and correcting defects early in the
development process.
---
## Selected Tool and GitHub Repository
#### I will be using ***mypy*** tool for static analysis.
#### GitHub Repository: https://github.com/ageitgey/face_recognition.git
---
## Installation of mypy
![image](https://user-images.githubusercontent.com/75067919/227470249-c2926225-db96-40ae-ba0f-3950d3ce21d7.png)
---

## Clone repository
![image](https://user-images.githubusercontent.com/75067919/227472897-845ba15d-cd20-4ae7-a1a3-359c770c14f7.png)
---

## Performing Static Analysis and Error Understanding
### 1. https://github.com/ageitgey/face_recognition/blob/master/face_recognition/face_recognition_cli.py
![image](https://user-images.githubusercontent.com/75067919/227474238-1eeda319-b2ee-42db-bee9-d52299c21e35.png)
### ***Understanding of errors***
* **As per the above photo, all 8 errors are of the importing modules which means mypy was able to find the module i was importing, but no corresponding type hints.** <br>
* **There are also 3 notes in the analysis. According to me, those notes is for hints or better implementations or some suggestions.**
* **In the 2nd note it is also giving commands to install missing stub packages.** <br>
### 2. https://github.com/ageitgey/face_recognition/blob/master/face_recognition/face_detection_cli.py
![image](https://user-images.githubusercontent.com/75067919/227475842-7a2b0aa7-4276-4862-b9a3-b4c0444079f7.png)
### ***Understanding of errors***
* **As same as the above file analysis, all 5 errors are of the importing modules.** <br>
* **There is also a note in the analysis which is suggesting to see the webpage for more information.** <br>
### 3. https://github.com/ageitgey/face_recognition/blob/master/face_recognition/api.py
![image](https://user-images.githubusercontent.com/75067919/227476099-eed5715a-f4a8-4b15-a008-0a148f3efca3.png)
### ***Understanding of errors***
* **In this analysis one error is different from above two analysis.** <br>
* **This error is saying that "PIL.image" and "PIL" library is not installed on the host machine.** <br>
### 4. https://github.com/ageitgey/face_recognition/blob/master/examples/face_recognition_knn.py
![image](https://user-images.githubusercontent.com/75067919/227477398-e02a1da4-6a1b-476a-894f-99bbb602ad80.png)
### ***Understanding of errors***
* **As per the above photo,3 errors are of the importing modules which means mypy was able to find the module.** <br>
* **In this analysis one error is saying that "PIL.image" and "PIL" library is not installed on the host machine.** <br>
### 5. https://github.com/ageitgey/face_recognition/blob/master/examples/facerec_ipcamera_knn.py
![image](https://user-images.githubusercontent.com/75067919/227477760-de728f1c-e365-4fe7-8b9a-d8af71b00968.png)
### ***Understanding of errors***
* **As per the above photo,5 errors are of the importing modules which means mypy was able to find the module.** <br>
* **In this analysis one error is saying that "PIL.image" and "PIL" library is not installed on the host machine.** 
* **In the note it is also giving commands to install missing stub packages.**<br>
---
