# Performance-Testing-with_Jmeter


I’ve completed performance test on frequently used API ```https://restful-booker.herokuapp.com```

# Download process of Apache-Jmeter

### **Prerequisite**

- Java Install

### **Process**

1. Check if Java Is Installed
- Open the command prompt
- Put the command java -version


  ![image](https://github.com/user-attachments/assets/1979e523-80be-481c-bcf7-806ce634b48b)

if you have Java installed in your system, the command will show that Java is installed, else, before going forward with the installation of JMeter, you must install Java. download java from [here](https://www.oracle.com/java/technologies/downloads/)


2. Download JMeter

   - To download JMeter go to the Apache JMeter website
```https://jmeter.apache.org/download_jmeter.cgi```

- On the website go to the binaries section and download the zip file
- Wait for the zip folder to be downloaded

3.  Install JMeter
   - Once the zip folder is downloaded, go to the folder location, and then extract the zip folder.
   - Once the folder is extracted go inside that folder and then go inside the bin folder.
   - In the bin folder open the jmeter.bat file


![image](https://github.com/user-attachments/assets/56f4d80d-5976-410b-aa99-60ce6d6f2ea5)


4. Clone this repository
```git clone https://github.com/itsnipa/performance-testing-jmeter.git ```

5. Open jmeter in CML. it will redirect you to jmeter GUI.

   
6. Go to file and click on Open

![image](https://github.com/user-attachments/assets/44631686-3d77-41ba-9c36-1adcda12c2ab)

7. choose jmx files from report folder and open jmx file

8. Enable the listeners and run the files and see the results

![image](https://github.com/user-attachments/assets/62d51143-7c8a-475e-9824-41d4e0394ef4)

  results:

![image](https://github.com/user-attachments/assets/426f05ba-7fc5-4255-b078-41e5c9de6e9d)




  ### **HTML report generate process**


1. Open command line in apache-jmeter folder and run this two command one after another. before run this commands go to jmeter and disable the listeners of the jmx files which you had enabled.

   ```
    jmeter -n -t test_plan_booking_collection_100user.jmx -l report\test_plan_booking_collection_100user.jtl
   ```
   ```
    jmeter -g report\test_plan_booking_collection_100user.jtl -o report\test_plan_booking_collection_100user.html
   ```


**HTML Summary Reports**

  - for 100 user


    ![image](https://github.com/user-attachments/assets/0b4fb9e5-abe1-4c1f-8102-348b2d8a2185)


 - for 200 user


   ![image](https://github.com/user-attachments/assets/0def7bdc-a34a-49ee-a5de-0fd71d388a19)


 - for 300 user


   ![image](https://github.com/user-attachments/assets/923202ae-112c-47f5-abc1-730023aaa569)




