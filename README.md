# The patient-specific arryhythmia recognition
- 特定使用者基於心電圖（ECG）信號的心律失常識別
- This project is the Graduation Project / Final Year Project (FYP) of Department of Computer and Information Science, Faculty of Science and Technology, University of Macau.

# Abstract
- At present, the medical equipment for the physical examination is very complete. There are various equipments in the hospital, including electrocardiogram, computed tomography, ultrasound, magnetic resonance imaging, etc. These devices are bulky and expensive to purchase, and the general public needs to go to a hospital or a specific clinic to check their physical condition.
- For our goal, we need to build a software to detect whether this person has heart disease. We hope that each user can quickly detect what potential heart disease they may have at a low cost, fast and simple risk.
- 目前，用於身體檢查的醫療設備非常齊全。 醫院中有各種設備，包括心電圖，計算機斷層掃描，超聲，磁共振成像等。這些設備體積龐大且購買昂貴，並且公眾需要去醫院或特定診所檢查身體狀況 。
- 為了實現我們的目標，我們需要構建一個軟件來檢測此人是否患有心髒病。 我們希望每個用戶都能以低成本，快速而簡單的風險快速檢測出他們可能患有的潛在心髒病。

# Training Database in our case
- PTB Diagnostic ECG Database - https://physionet.org/content/ptbdb/1.0.0/

# Environment Requirement
- OS: Windows / Linus / Mac OS ( this project developed in macOS catalina 10.15.3 & Ubuntu 18.04 LTS)
- Python Version: Python 3( Python 3.7.4 is recommanded)
- Others: Arduino IDE(version 1.8.12 is recommanded)
# Hardware Requirement
- Computer with required environment
- Arduino UNO R3 (with USB cable)
- AD8232 Heart Beat / ECG Collecting Shield (with sensors/electrodes)

# Python 3 library installation
 Library using pip to install:
  - jupyter
  - wfdb
  - pandas
  - numpy
  - glob2
  - tensorflow
  - matplotlib
  - math3
  - scikit-learn
  - joblib
  - pyserial
  - tkinter
- Windows command: 

      py -m pip install [library]


- Linux & Mac OS command:     
        
      pip install [library]
      
      
# For problem of tkinter installation problem in Linux:
    sudo apt-get install python3-tk

# For problem of serial port connection in Linux:
    sudo chmod 666 [port]
# Open ipynb file

    Windows: py -m jupyter notebook
    Linux & Mac OS: jupyter notebook

# Stop running Jupyter notebook

 - Windows: 
    
        py -m jupyter notebook stop
    
 - Linux & Mac OS: 
 
        jupyter notebook stop

# Open Program

- Arduino (Open with Arduino IDE):
      
      /src/arduino/ECG_arduino/ECG_arduino.ino

        
- Python (Open with Jupyter Notebook or Google Colaboratory)

        Training Model: /src/python/ECG_Prediction_SVM.ipynb
        GUI Identification Application: /src/python/ECG_GUI_App.ipynb

# Start and Running Program
Collecting ECG Signal (Arduino):
- Connect Arduino UNO R3 with AD8232 Heart Beat / ECG Collecting Shield to Computer with Arduino I
- Check the USB port is available
- Paste the sensors/electrodes on user's body
- Check the Serial Potter and Serial Monitor in Arduino IDE to see the signal value and graph respectively
- Collect the signal in Serial Potter and do the further process
 Training Model and GUI application (Python):
- Open the program with Jupyter Notebook or Google Colaboratory
- Check the paths in program
- If everything is fine, click "Kernel -> Restart and Run All"
- For GUI identification application, change and check the port of Arduino UNO everytime.

# Contact
Steven, WONG MENG HENG(ws28451912@gmail.com)
Yumi, SIN IAO MEI(yumi-o3o@hotmail.com)




